# A52s 5G Device Tree

## Reference

Fr3squ1nh0ROM uses the following open-source A52s 5G device tree as a reference:

**Original repository:**
https://github.com/salvogiangri/android_device_samsung_a52sxq

**Maintainer:** Salvo Giangri

The original repository is a **TWRP device tree for the Samsung Galaxy A52s 5G (a52sxq)** and is licensed under the Apache License 2.0.

## How Fr3squ1nh0ROM will use it

The original device tree will **not be treated as the final Fr3squ1nh0ROM device tree**.

Instead, it will be used as an open-source hardware reference and starting point for developing the A52s 5G device configuration required by Fr3squ1nh0ROM.

The project will adapt the relevant device configuration for:

* One UI 8.5
* Android 16
* Samsung Galaxy A52s 5G (SM-A528B / a52sxq)
* Linux 5.4.302 kernel
* Samsung hardware and device-specific components
* Display and 120 Hz operation
* Audio
* Wi-Fi and Bluetooth
* Cameras
* Fingerprint
* Sensors
* Telephony and 5G
* Power and thermal management
* SELinux and Android 16 compatibility

TWRP-specific components will not automatically be included in the final ROM device tree.

## Original Work

The original device tree and its associated files remain the work of their respective authors and contributors.

Fr3squ1nh0ROM will preserve applicable copyright notices and license requirements when adapting code from the original project.

Any modifications made specifically for Fr3squ1nh0ROM will be documented as project-specific changes.

## Device

| Property | Value                     |
| -------- | ------------------------- |
| Device   | Samsung Galaxy A52s 5G    |
| Model    | SM-A528B                  |
| Codename | a52sxq                    |
| SoC      | Qualcomm Snapdragon 778G  |
| GPU      | Adreno 642L               |
| Display  | 6.5" Super AMOLED, 120 Hz |
| Storage  | UFS 2.1                   |

## Important

This repository does **not** redistribute proprietary Samsung firmware, vendor blobs, modem firmware, or other proprietary components.

Those components are obtained and used separately during development where legally appropriate.

The goal is to gradually transform the reference device configuration into a clean, Android 16-compatible device tree for Fr3squ1nh0ROM.
