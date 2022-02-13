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
