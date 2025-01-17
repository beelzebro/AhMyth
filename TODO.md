## Client-Side TODO List:
- [ ] 01: Integrate Live Camera Preview Stream for the Client. 
#
- [ ] 02: Rewrite AhMyth Client using the original 
payload from `v1.0-beta.2` as the starting point.
#
- [ ] 03: Generate a valid signing certificate to bypass Play Protect. 
#
- [ ] 04: Create persistence for the AhMyth payload
#
- [ ] 05: Figure out how to give the client access to 
`storage/emulated` so we can access it when using the
FIle Manager in the AhMyth Server Victims Lab.
#
- [ ] 06: add USSD dialing and response view feature for the 
AhMyth client, requested by user from Issue [#97](https://github.com/Morsmalleo/AhMyth/issues/97)
#
- [ ] 07: Add the ability to screenshot victim device screen
to the AhMyth Client.
#
- [ ] 08: Add the ability to view the victim devices screen in 
real-time as well as the ability and option to screen record the live
victim screen view.
#
#
## Server-Side TODO List:

- [ ] 01: integrate a `Retry` button and function into AhMyth's APK Builder 
interface, that when clicked, initates the rebuilding and signing of 
the decompiled original APK that failed to build previously but with 
the exception of using the added argument for apktool `--use-aapt` or 
`--use-aapt2`.

- THIS IS HALF DONE! the rebuild function just needs to be 
integrated.
#
- [x] 02: Create a backup copy of AhMyth's `AndroidManifest.xml`
file, and store it in the newly created backup directory 
`AhMyth/AhMyth-Server/app/app/Factory/Vault` in order to 
restore AhMyth's original manifest file back to it's original 
state after being edited with custom permissions.

- This is done! It just needs to be updated to work with the
Constants.js file
# 
- [ ] 03: Stabilise Launcher Activity binding method

This is almost stable, just need to code in some functions
taken from *msfvenom*, then add a way to hook smali files that use the
`super` method instead of the `OnCreate` method. This shouldn't be to hard
thanks to `dana-at-cp/backdoor-apk`.
#
- [ ] 04: Explore other, more discrete options for the 
URL payload masker.
#
- [ ] 05: Integrate the function to Log apktool.jar and sign.jar 
errors to a text file for the GUI version of AhMyth.
#
- [ ] 06: Restyle the AhMyth Server using the following

      1. Glassmorphism 
      2. Side scrolling tabs instead of top scrolling tabs
      3. Icons to replace the Tab names
      4. Settings menu for UI style adjustments
      5. Dark theme
      6. AhMyth user account login - Default username will be `ahmyth` 
      and the default password will be `trojan`
#
- [ ] 07: Figure out why AhMyth is so unstable on 
Windows machines!
#
- [ ] 08: Build the Super hook, as well as the super hooking function for AhMyth
so AhMyth can backdoor APK's using the `super` method instead of
`OnCreate`
#
## Client-Server TODO List:

- [ ] 01: Update `socket.io-client 0.8.3` to 
`socket.io-client 2.0.1` for the AhMyth Client, 
in order for *Victim connections* to work when
updating `socket.io 2.4.2` to `socket.io 4.x` for
the AhMyth Server.
#
- [ ] 02: Integrate phone call recording for both the 
*AhMyth Client* & *AhMyth Server*, then find a way to
to reject the request from the *Server* to the *Client*
to record calls, only if there is no phone call in progress,
then find out how to have AhMyth print the error message 
`No phone call in progress!` when the request is rejected.
#
- [ ] 03: Integrate a keylogger for the Client, and then integrate
the Tab for it to be used as an option in the Victims Lab
for the Server.
#
- [ ] 04: Integrate Video Recording for the Client & Server. 
#
- [ ] 05: Add the function & permissions to delete files from Storage
on the Victim Device to the Client, then add the function & button to 
request the deletion of selected files from the Storage on the victim device.
