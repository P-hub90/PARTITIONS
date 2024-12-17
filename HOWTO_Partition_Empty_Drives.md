# How to Partition an Empty Drive into 3 Partitions and Format Them with NTFS

## Objective
This guide will show you how to partition an empty disk into three partitions and format them using the **NTFS** file system in **Windows**.

 I found an video that is highly relevant for partitioning an empty drive. You can see the full video: https://youtu.be/Svul8zeXjmw?feature=shared .

## Prerequisites:
- An empty or unallocated disk attached to your computer.
- Administrative privileges to manage disk configurations.

## Procedure

### Step 1: Open Disk Management

1. Right-click on **This PC** and select **Manage**.
2. In the **Computer Management** window, go to **Disk Management** under the **Storage** section.
https://youtu.be/Svul8zeXjmw?feature=shared

### Step 2: Locate the Empty Disk
- In the **Disk Management** window, locate the new disk that has **Unallocated** space.
  - The disk will appear as "Disk X" (where X is the disk number) and show "Unallocated" as the status.
    ![image](https://github.com/user-attachments/assets/a184facb-64e6-4341-9a1e-74ed88e75867)
     - If the disk is not initialized, you may need to initialize it first (more on that in Step 3).

### Step 3: Initialize the Disk (If Not Already Initialized)
1. If the disk is new and uninitialized, right-click on the **Unallocated** space and select **Initialize Disk**.
  
2. Choose either the **MBR** (Master Boot Record) or **GPT** (GUID Partition Table) partition style. **GPT** is recommended for modern systems.
3. Click **OK** to initialize the disk.
  ![image](https://github.com/user-attachments/assets/3668c596-3d14-4926-8ada-a48ed4f2cbbb)
 

### Step 4: Create the First Partition
1. Right-click on the **Unallocated** space of the initialized disk and select **New Simple Volume**.
    ![image](https://github.com/user-attachments/assets/cf40cb54-704f-4c0b-a83d-b138be7d69c8)
2. In the **New Simple Volume Wizard**, specify the size for the first partition.
   ![image](https://github.com/user-attachments/assets/c5878da7-bbb0-4253-bced-9d06d6e536b6)
3. Click **Next**.
4. Assign a drive letter, such as **E:**, and click **Next**.
   ![image](https://github.com/user-attachments/assets/85a441b2-eeab-41c3-9a56-561bbe7055b0)
5. In the **Format Partition** window:
   - Select **NTFS** for the file system.
   - Leave the **Allocation unit size** as **Default**.
   - Enter a **Volume label** (e.g., "Data1") or leave it as the default.
   - Check **Perform a quick format** (optional but faster).
     ![image](https://github.com/user-attachments/assets/bd11626b-44d6-4799-9194-29667e3cbebe)
6. Click **Next**, then **Finish**.

   Follow the step 4 twice to create second and third partitions.

### Step 7: Verify the Partitions
- Once all three partitions are created and formatted, they will appear in **This PC** (or **My Computer**) with the assigned drive letters (e.g., **E:, F:, G:**).
  ![image](https://github.com/user-attachments/assets/b1c9f8a3-faa2-40d8-bcb5-f9eb5bcd3538)
- You can verify the partitions in **Disk Management** by ensuring each partition has a **NTFS** file system and the appropriate size.

### Step 8: Format Additional Partitions (If Needed)
- If any partitions show as **RAW** or unformatted, right-click on the partition in **Disk Management** and select **Format**.
- Select **NTFS** and follow the formatting steps.

## Conclusion
You have successfully partitioned the empty drive into three partitions and formatted them using **NTFS**. These partitions are now ready for use.
