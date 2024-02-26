# Debloat

- Uninstalling unnecessary pre-installed applications and services, is a process that some users perform to optimize system performance and reduce its overall size. However, this process should be approached with caution because removing some components can affect the stability and functionality of the operating system. Make sure you understand the potential risks and back up important data before proceeding with this operation.
```
Powershell -command "Get-AppxPackage -allusers Microsoft.Wallet | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsAlarms | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsCalculator | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsCamera | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsFeedbackHub | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Disney.37853FC22B2CE | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.BingNews | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.BingWeather | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.GetHelp | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.Getstarted | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.Microsoft3DViewer | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.MicrosoftOfficeHub | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.MicrosoftSolitaireCollection | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.MicrosoftStickyNotes | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.MixedReality.Portal | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.MSPaint | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.Office.OneNote | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.OneDriveSync | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.People | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.PowerAutomateDesktop | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.ScreenSketch | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.SkypeApp | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.Todos | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsMaps | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.WindowsSoundRecorder | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.YourPhone | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.ZuneMusic | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers Microsoft.ZuneVideo | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers MicrosoftTeams | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers MicrosoftWindows.Client.WebExperience | Remove-AppxPackage"
Powershell -command "Get-AppxPackage *Microsoft.WebpImageExtension* | Remove-AppxPackage"
Powershell -command "Get-AppxPackage *Microsoft.WebMediaExtensions* | Remove-AppxPackage"
Powershell -command "Get-AppxPackage *Microsoft.Print3D* | Remove-AppxPackage"
Powershell -command "Get-AppxPackage *Microsoft.HEIFImageExtension* | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers SpotifyAB.SpotifyMusic | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers microsoft.windowscommunicationsapps | Remove-AppxPackage"
Powershell -command "Get-AppxPackage -allusers yandex | Remove-AppxPackage"
Powershell -command "Get-AppxPackage *Microsoft.549981C3F5F10* | Remove-AppxPackage"
Powershell -command "Get-WindowsPackage -Online | Where PackageName -like *Hello-Face* | Remove-WindowsPackage -Online -NoRestart"
Powershell -command "Get-WindowsPackage -Online | Where PackageName -like *QuickAssist* | Remove-WindowsPackage -Online -NoRestart"
%SystemRoot%\SysWOW64\OneDriveSetup.exe /uninstall
rd "%LocalAppData%\Microsoft\OneDrive" /Q /S
rd "%ProgramData%\Microsoft OneDrive" /Q /S
rd "C:\OneDriveTemp" /Q /S
REG Delete "HKEY_CLASSES_ROOT\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6}" /f
REG Delete "HKEY_CLASSES_ROOT\Wow6432Node\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6}" /f
```
