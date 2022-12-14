---
layout: wiki
title: Flash L5 Pro 3070 VBIOS on L5 3070
description: "Detailed and comprehensive guide on flashing the 140 W 3070 VBIOS from the 5 Pro to the Legion 5"
parent: Windows Guides
grand_parent: General
contributors: ['SweatyLaptopNerd']
discord: ⫶ ['nonkerdoob#0034']
---

# Flashing L5 Pro 3070 VBIOS on L5 3070

**Disclaimer: Flashing a BIOS always carries potential risks. You are the only responsible for what happens to your device.** 

- Go to ```BIOS –> Security –> Secure Boot```and disable it (This might be under boot for newer Legion models).
- Change the graphics mode to Hybrid, as the iGPU will be needed if this guide works for the worst (This is really important).
- Download the files provided and extract them into a folder.
- Open CMD as admin and change the directory of the extracted folder ```cd <Path to extracted folder>```
- Replace ```<Path to extracted folder>```. To get the path, open the folder in the file explorer and copy it from the adress bar.
- Run the following command to create a backup of the current VBIOS ```nvflash.exe -b 130w.rom```
- Run the following command to flash the new VBIOS ```nvflash.exe -f -6 140w.rom```
- Restart the device
- Ensure that everything is working as intended.

**Note**: To flash back the old vBIOS use the command ```nvflash.exe -f -6 130w.rom```
