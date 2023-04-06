# opencore-asus-rog-strix-b360-g-gaming-i5-8400
## My Hardware
**Mainboard**: ASUS ROG STRIX B360-G GAMING

**CPU**: Intel Core i5 8400

| Component     | Chipset                       | Is Work? |
| ------------- |-------------------------------|----------|
| Audio         | RealTek ALC S1220A            | YES      |
| LAN           | Intel I219-V                  | YES      |
| iGPU          | Intel UHD Graphics 630        | YES      |

## What did I do?
- Create SSDT-AWAC manually
- Create SSDT-PLUG manually
- Create SSDT-PMC manually
- Patch iGPU to work with HDMI

## Supported macOS versions

### Catalina 10.15.7

### Big Sur 11.7.5

### Ventura 13.3

## BIOS Setup

**MUST** in Advanced Mode

### Disable

- Fast Boot: Boot -> Fast Boot
- Secure Boot: Boot -> Secure Boot -> Key Management -> Clear
- Serial/COM Port: Advanced -> Onboard Device Configuration -> Serial Port
- Parallel Port: N/A
- VT-d: Advanced -> System Agent (SA) Configuration -> VT-d
- Compatibility Support Module (CSM): Boot -> CSM -> Launch
- Thunderbolt: N/A
- Intel SGX: Advanced -> CPU Configuration -> SGX
- Intel Platform Trust: N/A
- CFG Lock: Advanced -> CPU Configuration -> CPU - Power Management Control -> CFG Lock

### Enable

- VT-x: Supported
- Above 4G Decoding: Advanced -> PCI Subsystem Setting -> Above 4G Decoding
- Hyper Threading: Not Supported
- Execute Disable Bit: N/A
- EHCI/XHCI Hand-off: Advanced -> USB Configuration -> XHCI Hand-off
- OS Type: Boot -> Secure Boot -> OS Types -> Select `Other OS`
- DVMT Pre Allocated: Advanced -> System Agent (SA) Configuration -> Graphic Configuration ->  DVMT Pre Allocated -> Select `64 MB` or more
- SATA Mode: Advanced -> PCH Storage Configuration -> SATA Model -> Select `AHCI`
