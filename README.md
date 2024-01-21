# TWRP Tree for Xiaomi Mi MIX 2
```
#
# Copyright (C) 2012-2024 Team Win Recovery Project
#
# SPDX-License-Identifier: Apache-2.0
#
```

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core (4x2.45 GHz Kryo & 4x1.9 GHz Kryo)
Chipset | Qualcomm MSM8998 Snapdragon 835
GPU     | Adreno 540
Memory  | 6 GB RAM
Shipped Android Version | 7.1.1
Storage | 64/128 GB
Battery | Li-Po 3350 mAh battery
Display | 1080 x 2160 pixels, 5.99 inches (~403 ppi pixel density)
Rear Camera  | 12 MP, f/2.0, phase detection autofocus, dual-LED (dual tone) flash

## Device picture

![Xiaomi Mi MIX 2](https://i8.mifile.cn/a1/pms_1505401464.03824312!560x560.jpg "Xiaomi Mi MIX 2 in black")

## Kernel Source

https://github.com/Nanhumly-Staging/android_kernel_xiaomi_msm8998

## Compile

First repo init the TWRP 12.1 tree:

```shell
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
```

Sync source:

```shell
repo sync
```

Finally execute these:

```
.build/envsetup.sh
lunch twrp_chiron-eng
mka recoveryimage
```
