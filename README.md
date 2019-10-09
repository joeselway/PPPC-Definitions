# PPPC-Definitions

#### Below is a table mapping Apple's developer documentation for PPPC controls to the user GUI in macOS 10.15 Catalina

[Apple Dev Docs source: https://developer.apple.com/documentation/devicemanagement/privacypreferencespolicycontrol/services](https://developer.apple.com/documentation/devicemanagement/privacypreferencespolicycontrol/services)

S&P Prefs source: macOS 10.15.0 System Preferences > Security & Privacy

"Enabled" refers to when the app list is active, i.e. after an app has requested access, where the options is not always enabled.

"Always enabled" refers to options such as Accessibility which offer +/- buttons below an empty list

"Disabled" refers to when the GUI only presents a message regarding apps that have requested access appearing.

| Apple Dev Docs |   S&P Prefs   | Dev description | S&P description enabled | S&P description disabled | Notes |
|----------------|---------------|-----------------|-------------------------|--------------------------|-------|
| Accessibility | S&P Prefs | Specifies the policies for the app via the Accessibility subsystem. | Allow the apps below to control your computer. | *Always enabled*
| AddressBook | Contacts | Specifies the policies for contact information managed by the Contacts.app. | Allow the apps below to access your contacts. | Apps that have requested access to your contacts will appear here.
| AppleEvents | Automation | Specifies the policies for the app sending restricted AppleEvents to another process. | S&P description enabled | S&P description disabled
| Calendar | S&P Prefs | Specifies the policies for calendar information managed by the Calendar.app. | Allows the apps below to access your calendar. | Apps that have requested access to your calendar will appear here.
| Camera | S&P Prefs | A system camera. Access to the camera cannot be given in a profile; it can only be denied. | Allows the apps below to access your calendar. | Apps that have requested access to your camera will appear here.
| FileProviderPresence | S&P Prefs | Allow a File Provider application to know when the user is using files managed by the File Provider. | S&P description enabled | S&P description disabled
| ListenEvent | Input Monitoring | Allow the application to use CoreGraphics and HID APIs to listen to (receive) CGEvents and HID events from all processes. Access to these events cannot be given in a profile; it can only be denied. | Allow the apps below to monitor input from your keyboard even while using other apps. | Apps that have requested access to monitor input from your keyboard will appear here. | **Can add apps to list when enabled. Disabled when no apps in list**
| MediaLibrary | S&P Prefs | Allows the application to use CoreGraphics and HID APIs to listen to (receive) CGEvents and HID events from all processes. Access to these events cannot be given in a profile; it can only be denied. | S&P description enabled | S&P description disabled
| Microphone | S&P Prefs | A system microphone. Access to the microphone cannot be given in a profile; it can only be denied. | Allow the apps below to access your calendar. | S&P description disabled
| Photos | S&P Prefs | The pictures managed by the Photos app in ~/Pictures/.photoslibrary. | S&P description enabled | Apps that have requested access to your photos will appear here.
| PostEvent | S&P Prefs | Specifies the policies for the application to use CoreGraphics APIs to send CGEvents to the system event stream. | S&P description enabled | S&P description disabled
| Reminders | S&P Prefs | Specifies the policies for reminders information managed by the Reminders app. | Allow the apps below to access your reminders. | S&P description disabled
| ScreenCapture | Screen Recording | Allows the application to capture (read) the contents of the system display. Access to the contents cannot be given in a profile; it can only be denied. | Allow the apps below to record the contents of your screen, even while using other apps. | S&P description disabled
| SpeechRecognition | Speech Recognition | Allows the application to use the system Speech Recognition facility and to send speech data to Apple. | S&P description enabled | Apps that have requested access to speech recognition will appear here. Speech recognition sends recorded voice to Apple to process your requests | S&P description disabled
| SystemPolicyAllFiles | Full Disk Access | Allows the application access to all protected files, including system administration files. | Allows the application access to all protected files, including system administration files. | Allows the apps below to access data like Mail, Messages, Safari, Home, Time Machine backups and certain administrative settings for all users on this Mac. | S&P description disabled
| SystemPolicyDesktopFolder | Files and Folders   | Allows the application to access files in the user's Desktop folder. | S&P description enabled | S&P description disabled
| SystemPolicyDocumentsFolder |   Files and Folders   | Allows the application to access files in the user's Documents folder. | S&P description enabled | S&P description disabled
| SystemPolicyDownloadsFolder |   Files and Folders   | Allows the application to access files in the user's Downloads folder. | S&P description enabled | S&P description disabled
| SystemPolicyNetworkVolumes |   Files and Folders   | Allows the application to access files on network volumes. | S&P description enabled | S&P description disabled
| SystemPolicyRemovableVolumes |   Files and Folders   | Allows the application to access files on removable volumes. | S&P description enabled | S&P description disabled
| SystemPolicySysAdminFiles |   Files and Folders??   | Allows the application access to some files used in system administration. | S&P description enabled | S&P description disabled
| ???? | Developer Tools
| ???? | Advertising
| ???? | Analytics
