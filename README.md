# Mac-os-hackintosh-dell-7280
## opencore ,macOS Ventura beta 9
<img width="392" alt="Screenshot 2022-10-04 at 17 29 56" src="https://user-images.githubusercontent.com/52024444/193862158-7a3e44b8-56b4-40bf-81d5-2774ad8ce3c9.png">

## unlock CFG lock and DVMT are necessary if you use this EFI.Also need to modify Bios settings 
### how to do ?  
### Bios settings
Enable :
1. SATA Operation : AHCI.   2. Fastboot : Minimal.  3. Integrated NIC : Enable.
#### Disable :
1. Secure Boot.  2.Absolute.   3. Intel SGX.   4. Wake on AC.  5. Wake on Dell USB-C Dock.   6.Enable UEFI Network Stack.  7.VT-d. 

### unlock CFG lock and DVMT
#### For set CFG LOCK Disabled
#### setup_var 0x4ED 0x0

#### For set DVMT PRE Allocated to 64 MB
####  setup_var 0x795 0x2

#### For set DVMT Total GFX Mem to MAX
#### setup_var 0x796 0x3



## for intel wifi

## this efi need to inject SSN,UUID,ROM,MLB
