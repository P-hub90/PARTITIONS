# How to Add 2 Additional Drives to a Virtual Machine

 I found a video that is highly relevant for adding additional drives to a virtual machine. You can see the full video: https://youtu.be/KVX63ieQVjU?feature=shared.

## Objective

This document will guide you through the process of adding two additional virtual hard drives to an existing virtual machine (VM) in  Hyper-V.

## Prerequisites:

- A virtual machine is already created in Hyper-V.
- The virtual machine should be powered off before adding new disks.

## Procedure

### Step 1: Open Hyper-V Manager. 

### Step 2: Power Off the Virtual Machine

Before adding new hardware to the VM, you must ensure that the VM is powered off. In your hypervisor console:
Right-click on the VM and choose **Power Off** or **Shut Down**.


### Step 3: Add Additional Hard Drive

1. Right-click on the VM and choose **Settings**.
2. Under **Hardware**, click **Hard Drive**.
3. Select **Virtual hard disk** and click **New**.
   ![image](https://github.com/user-attachments/assets/61d786ae-65f8-43c6-bae3-94188e490930)
4. Define the name, size, location and type (VHD/VHDX) for the new disk.
   
5. Repeat the process to add the second disk. 
