# PPPC-Definitions

#### Below is a table mapping Apple's developer documentation for per-app PPPC controls to the user GUI in macOS 10.15 Catalina

Apple Dev Docs source: [https://developer.apple.com/documentation/devicemanagement/privacypreferencespolicycontrol/services](https://developer.apple.com/documentation/devicemanagement/privacypreferencespolicycontrol/services)

S&P Prefs source: macOS 10.15 (19A583) System Preferences > Security & Privacy

Profile options source: [Jamf PPPC-Utility v1.1.2](https://github.com/jamf/PPPC-Utility)

The "*Enabled*" description refers to when the app list is populated, i.e. after an app has requested access.

The "*Disabled*" description refers to when the GUI only presents a message regarding apps that have requested access appearing instead of an empty list.

"*Always enabled*" refers to options such as Accessibility which offer +/- buttons even when the list is empty.

| Apple Developer Docs | S&P PrefPane | Profiles PrefPane | Dev description | S&P description enabled | S&P description disabled | Profile options | Notes |
|----------------------|--------------|-------------------|-----------------|-------------------------|--------------------------|-----------------|-------|
| Accessibility | Accessibility | ???? | Specifies the policies for the app via the Accessibility subsystem. | Allow the apps below to control your computer. |  *Always enabled* | Allow/Deny |
| AddressBook | Contacts | ???? | Specifies the policies for contact information managed by the Contacts.app. | Allow the apps below to access your contacts. | Apps that have requested access to your contacts will appear here. | Allow/Deny |
| AppleEvents | Automation | ???? | Specifies the policies for the app sending restricted AppleEvents to another process. | S&P description enabled | S&P description disabled | Allow/Deny |
| Calendar | Calendar | ???? | Specifies the policies for calendar information managed by the Calendar.app. | Allows the apps below to access your calendar. | Apps that have requested access to your calendar will appear here. | Allow/Deny |
| Camera | Camera | ???? | A system camera. Access to the camera cannot be given in a profile; it can only be denied. | Allows the apps below to access your calendar. | Apps that have requested access to your camera will appear here. | **Deny only** |
| FileProviderPresence | ???? | ???? | Allow a File Provider application to know when the user is using files managed by the File Provider. | S&P description enabled | S&P description disabled | Allow/Deny |
| ListenEvent | Input Monitoring | ???? | Allow the application to use CoreGraphics and HID APIs to listen to (receive) CGEvents and HID events from all processes. Access to these events cannot be given in a profile; it can only be denied. | Allow the apps below to monitor input from your keyboard even while using other apps. | Apps that have requested access to monitor input from your keyboard will appear here. | **Deny only** | **Can add apps to list when enabled. Disabled when no apps in list**
| MediaLibrary | ???? | ???? | Allows the application to access Apple Music, music and video activity, and the media library. | S&P description enabled | S&P description disabled | Allow/Deny |
| Microphone | Microphone | ???? | A system microphone. Access to the microphone cannot be given in a profile; it can only be denied. | Allow the apps below to access your calendar. | S&P description disabled | **Deny only** |
| Photos | Photos | ???? | The pictures managed by the Photos app in ~/Pictures/.photoslibrary. | S&P description enabled | Apps that have requested access to your photos will appear here. | Allow/Deny |
| PostEvent | ???? | ???? | Specifies the policies for the application to use CoreGraphics APIs to send CGEvents to the system event stream. | S&P description enabled | S&P description disabled | Allow/Deny |
| Reminders | Reminders | ???? | Specifies the policies for reminders information managed by the Reminders app. | Allow the apps below to access your reminders. | S&P description disabled
| ScreenCapture | Screen Recording | ???? | Allows the application to capture (read) the contents of the system display. Access to the contents cannot be given in a profile; it can only be denied. | Allow the apps below to record the contents of your screen, even while using other apps. | S&P description disabled | **Deny only** |
| SpeechRecognition | Speech Recognition | ???? | Allows the application to use the system Speech Recognition facility and to send speech data to Apple. | S&P description enabled | Apps that have requested access to speech recognition will appear here. Speech recognition sends recorded voice to Apple to process your requests | **Deny only** |
| SystemPolicyAllFiles | Full Disk Access | Access All Application Data | Allows the application access to all protected files, including system administration files. | Allows the apps below to access data like Mail, Messages, Safari, Home, Time Machine backups and certain administrative settings for all users on this Mac. | ???? | Allow/Deny |
| SystemPolicyDesktopFolder | Files and Folders | ???? | Allows the application to access files in the user's Desktop folder. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| SystemPolicyDocumentsFolder | Files and Folders | ???? | Allows the application to access files in the user's Documents folder. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| SystemPolicyDownloadsFolder | Files and Folders | ???? | Allows the application to access files in the user's Downloads folder. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| SystemPolicyNetworkVolumes | Files and Folders | ???? | Allows the application to access files on network volumes. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| SystemPolicyRemovableVolumes | Files and Folders | ???? | Allows the application to access files on removable volumes. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| SystemPolicySysAdminFiles | Files and Folders | ???? | Allows the application access to some files used in system administration. | Allow the apps below to access files and folders. | ???? | Allow/Deny |
| ???? | Developer Tools | *Always enabled* |