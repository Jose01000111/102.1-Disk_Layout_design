# 💽 LPIC-1 Lab: Disk Layout Design 
# ⚠️ Note: This lab could not be fully completed due to a system-level issue that rendered the CentOS environment unstable. However, key concepts around partitioning, swap configuration, and LVM initialization were explored and partially tested. I plan to revisit and complete the lab after further investigation and environment restoration
## 📝 Introduction
In this lab, I designed a disk partitioning layout for a Linux system, tailored to meet different use cases and hardware requirements. I practiced allocating key filesystems to different partitions, understanding swap space, and working with LVM and EFI system partitions.

I’ve included some helpful links to guide you through the lab and for studying afterward:

[Ojective 102.1](https://www.lpi.org/our-certifications/exam-101-102-objectives/#102.1_Design_hard_disk_layout)

[Objective 102.1 Notes](https://1drv.ms/w/c/354f1c8d534fbced/EbMbgOosyTNGqT0F4gN5mQABwJOvi-IWub3HHxZX1hBwUA?e=zGLqhj)

[Objective 102.1 Lab](https://1drv.ms/w/c/354f1c8d534fbced/ERuF45SgDZJLuDj3YtOo67QBysILXQFi-YnuFxlJsUz96Q?e=14RDgm)

---

## 🚀 What I Did in This Lab
I simulated creating and planning a disk layout for a Linux system using fdisk, lsblk, and logical volume tools. I also reviewed architecture-specific boot requirements and explained my design choices.

## 1️⃣: Allocate Filesystems and Swap to Separate Partitions

I started by learning how to divide the disk into multiple partitions, assigning directories like /, /boot, /home, and /var to separate filesystems and setting up swap space appropriately.

🔹Identify Available Disks

🔹Create Basic Partitions with fdisk

![Y96Wv8G](https://github.com/user-attachments/assets/57d50501-f948-4cb1-930e-247e1409e3d2)

🔹Format and Mount Partitions

![12ZDDz7](https://github.com/user-attachments/assets/18c8a777-0123-4cbb-bfe3-953405230d7c)

---

![Rk2Rn58](https://github.com/user-attachments/assets/6da69803-4302-4df7-b7cf-d7c481a85f3b)

---

![eBf1ktP](https://github.com/user-attachments/assets/93b40dac-8ffb-4a99-947b-c2c9bf9fa340)

## 2️⃣: Understand Basic Features of LVM 

Finally, I explored Logical Volume Management (LVM), learning how to create physical volumes, volume groups, and logical volumes to make storage more flexible and scalable.

🔹 Initialize LVM Components

🔹 Create and Mount Logical Volumes

![mchJ4u8](https://github.com/user-attachments/assets/8336bc45-d1b5-4f03-a06e-a274f3961914)

## 📚 What I Learned
👨‍💻 I gained valuable hands-on experience in designing a flexible and role-specific disk layout. I manually created partitions, configured swap space, and explored LVM for dynamic storage management. While experimenting with different layouts and boot configurations, I mispartitioned the disk and incorrectly configured the layout, which ultimately compromised the CentOS environment. Despite the issue, I developed a deeper understanding of the boot process, EFI partitioning, and the importance of precise disk planning. I plan to revisit this lab after rebuilding the environment to reinforce and apply what I’ve learned. 🧰🐧
