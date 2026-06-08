Ubuntu Boot Freeze Troubleshooting

Overview

This document describes the installation and troubleshooting process of Ubuntu on a Lenovo V15 G2 ITL laptop.

System Information

- Device: Lenovo V15 G2 ITL
- BIOS Version: GGCN61WW
- Operating System: Ubuntu 24.04.5 LTS
- Installation Type: Dual Boot (Windows + Ubuntu)

Problem

Ubuntu repeatedly froze during boot after being selected from GRUB.

Observed symptoms:

- Freeze during boot process
- ACPI-related messages before system lockup
- Similar behavior in multiple Linux distributions

Investigation

The following troubleshooting steps were performed:

- BIOS inspection
- Memory testing
- Live USB testing
- Kernel parameter experimentation

Tested parameters:

- nomodeset
- acpi=off
- noapic

None of the above resolved the issue but this one : 
- irqpoll acpi-osi=! acpi-osi="Windows 2020"

Solution

The following kernel parameters allowed Ubuntu to boot successfully:

irqpoll acpi_osi=! acpi_osi="Windows 2020"

The parameters were permanently added to GRUB configuration.

Result

- Ubuntu boots successfully
- Dual boot configuration remains functional
- Manual GRUB editing is no longer required

Lessons Learned

- Firmware compatibility issues may affect Linux even when Windows works correctly.
- Kernel boot parameters can be critical during troubleshooting.
- Systematic testing helps isolate root causes efficiently.
