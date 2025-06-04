# 💽 LPIC-1 Lab: Disk Layout Design

## 📝 Introduction
In this lab, I designed a disk partitioning layout for a Linux system, tailored to meet different use cases and hardware requirements. I practiced allocating key filesystems to different partitions, understanding swap space, and working with LVM and EFI system partitions.

## 🚀 What I Did in This Lab
I simulated creating and planning a disk layout for a Linux system using fdisk, lsblk, and logical volume tools. I also reviewed architecture-specific boot requirements and explained my design choices.

## 1️⃣: Allocate Filesystems and Swap to Separate Partitions

I started by learning how to divide the disk into multiple partitions, assigning directories like /, /boot, /home, and /var to separate filesystems and setting up swap space appropriately.

🔹Identify Available Disks

🔹Create Basic Partitions with fdisk

🔹Format and Mount Partitions

## 2️⃣: Tailor Layout to Intended System Use: 

Next, I adapted the partition scheme based on how the system would be used—for example, increasing /var for a web server or expanding /home for a developer environment.

🔹Web Server: Larger /var for logs, cache, and web files

🔹Developer Workstation: Larger /home for personal files

🔹Minimal System: Single / with fewer partitions for simplicity

## 3️⃣: Ensure /boot Meets Architecture Requirements: 

I then focused on configuring the /boot partition to meet BIOS and UEFI requirements, including creating an EFI System Partition when needed for modern hardware.

🔹BIOS: /boot within first 2TB of disk

🔹UEFI: Create EFI System Partition

## 4️⃣: Understand Basic Features of LVM 

Finally, I explored Logical Volume Management (LVM), learning how to create physical volumes, volume groups, and logical volumes to make storage more flexible and scalable.

🔹 Initialize LVM Components

🔹 Create and Mount Logical Volumes

## 📚 What I Learned
👨‍💻 I learned how to design a flexible and efficient disk layout based on the system’s role. I practiced creating partitions manually, managing swap space, and using LVM for flexible storage. I also gained insight into the boot process and EFI partitioning! 🧰🐧
