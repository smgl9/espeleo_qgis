---

header:  -[Index](./index.html#1)-
footer:  Hassio vbox installation guide --  [pdf slides](./vbox.pdf)
marp: true
title: Hassio vbox installation guide
description: How to install the tools in virtualbox
theme: uncover
paginate: true
_paginate: false

---

<style scoped>{text-align: left;}</style> 
### Vbox
- Install VirtualBox: [Vbox](https://www.virtualbox.org/)
- Download VirtualBox (VDI) hassio image: [hassio](https://www.home-assistant.io/installation/windows)

---

<style scoped>{text-align: left;font-size: 30px;}</style>  
### Create the virtual machine

Minimum recommended assignments:
- 2 GB RAM
- 32 GB Storage
- 2vCPU

---

<style scoped>{text-align: left;font-size: 30px;}</style> 
### Hypervisor configuration:

  - Create a new virtual machine.
  - Select type Linux and version Linux 2.6 / 3.x / 4.x (64-bit).
  - Select Use an existing virtual hard disk file, select the unzipped VDI file from above.
  - Edit the Settings of the VM and go to System > Motherboard. Select Enable EFI.
  - Then go to Network > Adapter 1. Choose Bridged Adapter and choose your network adapter.

---
<style scoped>{text-align: left;font-size: 30px;}</style> 
### Start up your virtual machine

  - Start the virtual machine.
  - Observe the boot process of the Home Assistant Operating System.
  - Once completed, you will be able to reach Home Assistant on homeassistant.local:8123. Ifyou are running an older Windows version or have a stricter network configuration, you might need to access Home Assistant at homeassistant:8123 or http://X.X.X.X:8123(replace X.X.X.X with your ’s IP address).


---
