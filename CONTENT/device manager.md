# Device Manager


- Access Device Manager (devmgmt.msc) and deactivate any hardware components or drivers that are not currently in use. Exercise caution to avoid disabling anything essential. It's worth noting that uninstalling drivers via Device Manager may lead to their automatic reinstallation upon reboot. To fully prevent a driver from functioning, it's better to disable it rather than uninstalling it. Disabling a device or driver in Device Manager unloads it, preventing it from interrupting the CPU and potentially causing system slowdowns or interruptions due to poorly programmed drivers.

### What to disable:
```
Intel graphics (if you don’t use it, ideally should be disabled in the BIOS)
Microsoft ISATAP Adapter
Microsoft iSCSI Initiator
Composite Bus Enumerator
Intel Management Engine / AMD PSP
Intel SPI (flash) Controller
Microsoft GS Wavetable Synth
Microsoft Virtual Drive Enumerator (if not using virtual drives)
NDIS Virtual Network Adapter Enumerator
Remote Desktop Device Redirector Bus
SMBus
System speaker
Terminal Server Mouse/Keyboard drivers
UMBus
``` 
