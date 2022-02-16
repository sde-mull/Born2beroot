# What is an OS Kernel?

## Definition

-> The Kernel is **the most important part of the operating system.** It is the **primary interface** between the hardware and the processes of a computer. The Kernel connects these two in order to adjust resources as effectively as possible.

-> It is named a Kernel because it operates inside the OS, just like a seed inside a hard shell. It controls all of the main functions of the hardware, whether it's a tablet, desktop, server, or any kind of device.

-> **The Kernel is one of the initial programs** loaded up on memory before the boot loader. The boot loader is responsible for translating instructions for the central processing unit. It manages memory as well as peripherals such as keyboards and monitors.

## Purposes of the Kernel

-> The Kernel has several important jobs, such as process and memory management, disk storage, and low-level networking. We can summarize the main purposes of the Kernel as below:

   1. Determines which process is the next process on the central process unit (CPU), when, and how long.
   2. Monitors how much memory is being used to store what and where.
   3. Serves as an interpreter between the hardware and processes.
   4. Receives requests for service from the processes via system calls.

If the developers implement the Kernel appropriately, it is out of sight of the user. **It operates in its own area called the Kernel space.** It allocates memory and monitors where everything is stored in the Kernel space.

**The user space** is the environment where the user sees files and web browsers. These programs communicate with the Kernel using a system call interface.

## Where is the Kernel?

-> If we try to vizualize where the Kernel fits in a machine, we can think of the machine as having three layers:

![imagem](https://user-images.githubusercontent.com/78042197/153772972-2acc086d-0d5d-496b-813b-7cc0fff3a8ee.png)

**User Processes:** User processes actually create the userspace. However, these processes are the applications that the Kernel controls. The Kernel also enables these processes to communicate with each other. It uses inter-process communication (IPC) mechanisms to enable communication between processes.

**Kernel:** As we can see, it's right in the middle of the layers. **It's the core of the OS.**

**Hardware:** It's the physical machine, the base of the system. It consists of memory, the processor or the central processing unit (CPU), and input/output(I/O) components such as graphics, storage, and networking. The CPU executes computations, reads and writes memory.

**There are two modes for the code executed by the system on a CPU: Kernel mode and user mode.** While the code is running in Kernel mode, it has unlimited access to the hardware. However, if the code is running in user mode, it has limited access to the CPU and the memory.

These two modes provide some critical and complicated operations. For example, **it helps privilege separation for security.** Actually, this means that if a process fails in user mode, Kernel mode minimizes the error, and it can recover the process.

There are so many Kernel types, such as the **monolithic Kernel, microkernel, exokernel, hybrid Kernel, and nano Kernel.** The main difference between the monolithic kernel and microkernel is related to the system calls and their Kernel spaces.

For example, most Unix Kernels are monolithic. Each Kernel layer integrates into the entire Kernel program and runs in Kernel mode. On the other hand, microkernel operating systems only require a small number of kernel functions such as an IpC mechanism and, a basic scheduler.

# Primary Partition vs Logical partition

-> A hard disk drive can be divided in to several storage units. These storage units are called partitions. Creating partitions would make a single physical disk drive appear as multiple disks. Software that can be used to create, delete and modify partitions is called a partition editor. Creating partitions would allow the user filles to be resided separately from the operating system and other program files. Furthermore, partitions would allow the user to have multiple operating systems to be installed in different partitions of the same hard disk. Initially, a hard disk drive could be divided in to two partitions called the primary partition and extended partition. The extended partition could be further divided in to multiple logical drives. Information about the partitions in a computer is included in the partition table, which is located in the Master Boot Record (MBR).

![imagem](https://user-images.githubusercontent.com/78042197/153778635-b54f68a2-128a-4262-976f-80d30ff4e17b.png)

## What is Primary Partition?

-> A disk drive can contain a maximum of four primary partitions or three primary partitions and a single extended partition. One file system is contained in a primary partition. Unlike earlier versions of Microsoft Windows Systems, more recent Windows operating systems such as windows XP, windows 7 could be placed on any partition. But the boot files should be located in a primary partition. Partition type code of a primary partitions indicates information about the file system contained in the primary partition or the whether the partition has a special usage. When there are multiple primary partitions in a hard disk, only a single partition can be active at any given time and the other partitions will be hidden. If a drive needs to be bootable, it needs to be a primary partition.

## What is a Logical Partition?

-> The extended partition in a hard disk drive could be subdivided in to several partitions called logical partitions. The extended partition acts as a container for logical partitions. The structure of the logical portions in the extended partition is described using one or more Extended Boot Records(EBR). EBRs that describe multiple logical drives are organized as linked list. Each EBR comes before the logical drive described by it. The first EBR will contain the starting point of the EBR that describes the next logical drive. After the logical partitions are formatted using a suitable file system they will become visible.

## What is the difference between Primary Partition and Logical Partition?

-> Primary partition is a bootable partition and it contains the operating system/s of the computer, while logical partition is a partition that is not bootable. Multiple logical partitions allow storing data in an organized manner. Multiple primary partitions in a hard disk drive are described using a single partition table that is contained in the MBR, while multiple logical drives in hard disk drive are described using multiple EBRs. Due to this reason the number of primary partitions that could be created in a hard disk is limited (maximum is four), whereas the number of logical drives that could be created is limited only by the available hard disk space. Generally, primary partitions are assigned the first letters in the alphabet as drive letters(such as C,D) whereas logical drives get the other letters(such as E, F, G).
