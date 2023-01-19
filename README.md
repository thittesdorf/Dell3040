# Dell3040
Opencore Configuration for Dell 3040 Micro

Mostly working configuration for booting MacOS on a Dell 3040 Micro

![Dell 3040 Micro](https://i.dell.com/is/image/dellcontent//content/dam/ss2/product-images/dell-client-products/desktops/optiplex-desktops/optiplex-3040/micro/global-spi/desktop-optiplex-3040-micro-black-left-bestof-500-ng.psd?fmt=png-alpha&wid=200&hei=200&fit=constrain,1 "Dell 3040 Micro" )

## What isn't working
- Top USB port on front
- Some sleep states

## BIOS Settings

- General
    - System Information
        - BIOS 1.20.1
    - Boot Sequence
        - May need to delete Boot Options after OpenCore upgrades
    - Advanced Boot Options
        - Enable Legacy Options ROMs - Yes
        - Enable Attempt Legacy Boot - No
    - UEFI Boot Path Security
        - Never
- System Configuration
    - Integrated NIC
        - Enable UEFI Network Stack - No
        - Enabled
    - SATA Operation
        - AHCI
    - Drives
        - SATA-0 - Yes
    - SMART Reporting
        - Enable SMART Reporting - No
    - USB Configuration
        - Enable Boot Support - Yes
        - Enable Front USB Ports - Yes
        - Enable Rear USB Ports - Yes
    - Front USB Configuration
        - Front Port 1 (Bottom) - Yes
        - Front Port 2 (Top) - Yes ***This Port Doesn't Work***
    - Rear USB Configuration
        - Rear Port 1 (Bottom) - Yes
        - Rear Port 2 (Lower Middle) - Yes
        - Rear Port 3 (Upper Middle) - Yes
        - Rear Port 4 (Top) - Yes
    - Audio
        - Enable Audio - Yes
            - Enable Microphone - Yes
            - Enable Internal Speaker - Yes
- Video
    - Primary Display
        - Auto
- Security
    - UEFI Capsule Firmware Updates
        - Enable UEFI Capsule Firmware Updates - Yes
    - TPM 2.0 Security
        - TPM On - No
    - CPU XD Support
        - Enable CPU XD Support - Yes
    - SSM Security Mitigation
        - SSM Security Mitigation - Yes
- Secure Boot
    - Secure Boot Enable
        - Disabled
    - Expert Key Management
        - Enable Custom Mode - No
- Intel Software Guard Extensions
    - Intel SGX Enable
        - Disabled
- Performance
    - Multi Core Support
        - All
    - Intel SpeedStep
        - Enable Intel SpeedStep
    - C-States Control
        - C states - Yes
    - Limit CPUID Value
        - Enable CPUID Limit - No
    - Intel TurboBoost
        - Enable Itnel TurboBoost - Yes
- Power Management
    - Deep Sleep Control
        - Disabled
    - USB Wake Support
        - Enable USB Wake Support - No
    - Wake on LAN/WLAN
        - Disabled
    - Block Sleep
        - Block Sleep (S3 State) - No
    - Intel Ready Mode
        - Enable Intel Ready Mode - No
- POST Behavior
    - Fastboot
        - Thorough
- Virtualization Support
    - Virtualization Support
        - Enable Intel Virtualization Technology
    - VT for Direct I/O
        - Enable VT for Direct I/O - No
- Wireless
    - Wireless Device Enable
        - WLAN/WiGig - Yes
        - Bluetooth - Yes
        