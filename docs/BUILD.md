# Building Fr3squ1nh0ROM

## Overview

Fr3squ1nh0ROM is a community-driven project focused on adapting Samsung One UI 8.5 based on Android 16 to the Samsung Galaxy A52s 5G (SM-A528B / a52sxq).

The build environment and compilation process are still under development.

This document will be updated as the project progresses and the build system becomes reproducible.

## Target Device

| Property | Value                    |
| -------- | ------------------------ |
| Device   | Samsung Galaxy A52s 5G   |
| Model    | SM-A528B                 |
| Codename | a52sxq                   |
| SoC      | Qualcomm Snapdragon 778G |
| Android  | 16                       |
| One UI   | 8.5                      |

## Main Components

Fr3squ1nh0ROM is built around several major components:

### Kernel

The project uses the **Nova-Kernel** source as the kernel reference for the A52s 5G.

Kernel source:

https://github.com/m52xq/Nova-Kernel

The kernel is maintained separately from this repository.

### Device Tree

The A52s 5G device configuration is being developed using the following open-source device tree as a reference:

https://github.com/salvogiangri/android_device_samsung_a52sxq

The original project is a TWRP device tree. Relevant hardware configuration will be adapted for the Android 16 / One UI 8.5 environment used by Fr3squ1nh0ROM.

See [DEVICE_TREE.md](DEVICE_TREE.md) for more information.

## Proprietary Components

Fr3squ1nh0ROM does not redistribute proprietary Samsung components through this repository.

This includes, but is not limited to:

* Samsung firmware
* Proprietary vendor blobs
* Modem firmware
* Samsung applications
* Samsung framework components
* Proprietary libraries
* Device-specific proprietary binaries

Required proprietary components will be obtained separately during development where appropriate.

## Build Environment

The final build environment has not yet been frozen.

The project is expected to require a Linux-based development environment with the appropriate Android build tools, Java environment, compiler toolchains and supporting utilities.

Exact versions will be documented once the build system is finalized.

## Development Workflow

The intended development workflow is:

1. Prepare the Android 16 / One UI 8.5 base.
2. Prepare the A52s 5G device configuration.
3. Integrate the A52s-specific kernel.
4. Integrate the required hardware configuration and proprietary components locally.
5. Adapt `system`, `product` and `system_ext` for the A52s 5G.
6. Build the required images.
7. Boot and debug on the SM-A528B.
8. Fix hardware and framework compatibility issues.
9. Improve stability, thermal behavior and power management.
10. Validate SELinux and system integrity.
11. Produce internal test builds.
12. Progress toward Alpha, Beta and Stable releases.

## Current Status

**Status: Early Development**

The build system is not yet considered reproducible.

Hardware bring-up, system adaptation and build requirements are still being developed.

Do not expect a flashable public ROM from this repository yet.

## Notes

This project is intended for development and research purposes.

Always maintain backups when testing custom software on the device.

Fr3squ1nh0ROM is an independent community project and is not affiliated with or endorsed by Samsung Electronics.
