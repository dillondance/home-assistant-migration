# Implementation notes

## Source system
- Raspberry Pi 4 hosting Home Assistant OS from an SD card.
- Existing Home Assistant environment and connected devices needed to remain available after migration.

## Destination system
- UGREEN NASync DXP4800 Plus running a virtual machine with a Home Assistant OS QCOW2 image.
- Virtual networking used a VirtIO adapter during VM setup.
- Additional virtual hardware settings included USB controllers/devices and a serial interface.

## High-level procedure
1. Ensure a usable Home Assistant backup exists before migration.
2. Create the VM and attach the HAOS QCOW2 disk image.
3. Boot and wait for the Home Assistant command-line interface to indicate readiness.
4. Open the application in a browser and initiate restoration.
5. If the restore UI appears to hang, verify access in a separate tab rather than repeatedly restarting the VM.
6. Configure hardware passthrough only while the VM is in a state that allows virtual hardware changes.
7. Verify that serial-backed integrations and connected devices function.
8. Observe both VM-level allocation and application-reported usage.

## Boundaries of this case study
Exact VM specifications, integration names, physical device identifiers, IP addresses, secrets, and backup contents are intentionally not disclosed. This is an operational narrative, not a directly reusable, environment-specific deployment script.
