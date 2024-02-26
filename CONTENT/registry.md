# Customizing Optimal Registry Settings

- Customizing optimal registry settings and cleaning up your Windows system through the registry editor can improve the performance and stability of your operating system. However, you need to be careful when making changes to the registry, as incorrect settings can lead to undesirable consequences. It is recommended to create a restore point before making changes.

```
Windows Registry Editor Version 5.00

;Automatic Mainenance Disable
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Schedule\Maintenance]
"MaintenanceDisabled"=dword:00000001

;Disable Mouse Keys
[HKEY_CURRENT_USER\Control Panel\Accessibility\MouseKeys]
"Flags"="0"

;Disable Sticky Keys
[HKEY_CURRENT_USER\Control Panel\Accessibility\StickyKeys]
"Flags"="0"

;Disable Keyboard Response
[HKEY_CURRENT_USER\Control Panel\Accessibility\Keyboard Response]
"Flags"="0"

;Disabel Toggle Keys
[HKEY_CURRENT_USER\Control Panel\Accessibility\ToggleKeys]
"Flags"="0"

;Network Settings
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile]
"NetworkThrottlingIndex"=dword:0000000a
"SystemResponsiveness"=dword:0000000a

;Disable UAC
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System]
"EnableVirtualization"=dword:00000000
"EnableInstallerDetection"=dword:00000000
"PromptOnSecureDesktop"=dword:00000000
"EnableLUA"=dword:00000000
"EnableSecureUIAPaths"=dword:00000000
"ConsentPromptBehaviorAdmin"=dword:00000000
"ValidateAdminCodeSignatures"=dword:00000000
"EnableUIADesktopToggle"=dword:00000000
"ConsentPromptBehaviorUser"=dword:00000000
"FilterAdministratorToken"=dword:00000000


;Allow users to enable online speech recognition services
[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\InputPersonalization]
"AllowInputPersonalization"=dword:00000000

;Turn off automatic learning
[HKEY_CURRENT_USER\SOFTWARE\Policies\Microsoft\InputPersonalization]
"RestrictImplicitInkCollection"=dword:00000001
"RestrictImplicitTextCollection"=dword:00000001

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\InputPersonalization]
"RestrictImplicitInkCollection"=dword:00000001
"RestrictImplicitTextCollection"=dword:00000001

;Getting to know you
[HKEY_CURRENT_USER\Software\Microsoft\InputPersonalization]
"RestrictImplicitInkCollection"=dword:00000001
"RestrictImplicitTextCollection"=dword:00000001

[HKEY_CURRENT_USER\Software\Microsoft\InputPersonalization\TrainedDataStore]
"HarvestContacts"=dword:00000000

[HKEY_CURRENT_USER\Software\Microsoft\Personalization\Settings]
"AcceptedPrivacyPolicy"=dword:00000000

[HKEY_CURRENT_USER\Control Panel\Desktop]
"CursorBlinkRate"="-1"

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\services\NetBT]
"Start"=dword:00000004

[HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\PriorityControl]
"Win32PrioritySeparation"=dword:00000002

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\services\NDIS\Parameters]
"TrackNblOwner"=dword:00000000
```
