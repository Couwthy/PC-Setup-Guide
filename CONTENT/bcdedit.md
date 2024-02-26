# BCDEDIT
- Do not touch settings like useplatformclock, useplatformtick, disabledymanictick, tscsyncpolicy, they are designed for debugging and the system automatically installs them correctly. No need to force the timer to work, just leave it.
```
bcdedit /set firstmegabytepolicy     UseAll
bcdedit /set avoidlowmemory          0x8000000
bcdedit /set configaccesspolicy      Default
bcdedit /set displaymessageoverride  Recovery
bcdedit /set recoveryenabled         Yes
bcdedit /set noumex                  Yes
bcdedit /set vm                      No
bcdedit /set bootems                 No
bcdedit /set nointegritychecks       No
bcdedit /set testsigning             No
bcdedit /set extendedinput           Yes
bcdedit /set highestmode             Yes
bcdedit /set isolatedcontext         No
bcdedit /set forcefipscrypto         No
bcdedit /set allowedinmemorysettings 0x0
bcdedit /set nx                      AlwaysOff
bcdedit /set pae                     ForceEnable
bcdedit /set perfmem                 0
bcdedit /set x2apicpolicy            Enable
bcdedit /set msi                     Default
bcdedit /set bootmenupolicy          Legacy
bcdedit /set hypervisorlaunchtype    Off
bcdedit /set bootux                  Disabled
bcdedit /set tpmbootentropy          ForceDisable
bcdedit /set vsmlaunchtype           Off
bcdedit /set nolowmem                Yes
bcdedit /set usephysicaldestination  No
bcdedit /set onecpu                  No
bcdedit /set maxproc                 Yes
bcdedit /set usefirmwarepcisettings  No
bcdedit /set halbreakpoint           No
bcdedit /set ems                     No
```
