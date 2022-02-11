# Concepts

## How a virtual machine works?

-> Virtual machines are made possible through virtualization technology. Virtualization uses software to simulate virtual hardware that allows multiple VMs to run in a single machine. Thephysical machine is known as the host while the VMs running on it are called guests.

-> This process is managed by software known as hypervisor. The hypervisor is responsible for managing and provising resources (like memory and storage) from the host to guest. It also schedules operations in VMs so they don't overrun each other when using resources.

-> There are two types of hypervisors used in virtualization:
   1. Type 1 hypervisors are installed natively on the underlying physical hardware. VMs interact directly with hosts to allocate hardware resources without any           extra software layers in between. Host machines running type 1 hypervisors are used only for virtualization. They're often found in server based enviroments         like enterprise datacenters. A seperate management tool is needed to handle guest activities like creating new virtual machine instances or managing                 permissions.
   
   2. Type 2 hypervisors run on the host computer's operating system. Hosted hypervisors pass VM requests to the host operating system, which then provisions the       appropriate physical resources to each guest. Type 2 hypervisors are slower than their type 1 counterparts as every VM action has to go through the host             operating system first. Unlike type 1 (bare-metal hypervisors), guest operating systems are not tied to physical hardware. Users can run VMs and use their           computer system as usual. This makes type 2 (hosted hypervisors) suitable for personal users or small businesses that don't have dedicated servers for               virtualization.

## What is Hardware virtualization?

-> Hardware virtualization is the method used to create virtual versions of physical desktops and operating systems. It uses a virtual machine manager (VMM) called a hypervisor to provide abstracted hardware to multiple guest operating systems, which can then share the physical hardware resources more effenciently. Hardware virtualization offers many benefits, such as better performance and lower cost.

## What is a hypervisor?

-> A hypervisor is a software that creates and runs virtual machines, which are software emulations of a computing hardware environment. Sometimes called a virtual machine monitor(VMM), the hypervisor isolates the operating system and computing resources from the virtual machines and enables the creation and management of those VMs. These virtual machines - simply, code operating in a server's memory space - enable administrators to have a dedicated machine for every service they need to run.

-> This small software layer is the most important component of virtualization technology, which comprises storage, desktop, operating system and application virtualization. Hypervisors also make server virtualization possible by allowing different operating systems to run seperate applications on a single server while still using the same physical hardware resources. Virtualization is the basis of modern cloud computing, enabling scalability, security and management of global IT infrastructure.

## What is Debian?

-> Debian is considered to be the oldest linux-based distribution as it was launched in 1993. It is an open-source operating system created by individuals with common interests to develop this free OS.

-> Debian ensures **security and stability** to your system. Debian uses two types of kernels - Linux kernel and FreeBSD kernel. Debian is a commonly used OS for personal and network servers and is a base for other Linux distributions.

## Features of Debian

  1. Debian server comes with a wide range of installers as compared to other distributions.
  2. Its community meber still maintain Debian.
  3. It comes with an easy installation package.
  4. With Debian, you can use any software available for distribution.
  5. Debian supports multiple hardware architectures.
  6. Debian can be easily transitioned between new and old technologies.
  7. Debian comes with well-integrated packages.
  8. It adapts easily during an upgrade to the new release.
  9. Debian is by far the most secure and stable linux distribution available to date. It has a bug tracking system to resolve issues.

## Advantages of Debian

  1. As Debian is the oldest version, it has a much mature community.
  2. Debian's tested version is as stable as other distributions, and even Debian's stable distribution is rock-solid stable.
  3. Debian offers the largest repository for the software as compared to any other distribution.
  4. Debian's tools intend to do recursive system upgrades.
  5. The Debian package will notify you to install another package if required for working.
  6. The system works on a policy that allows it to maintain the distribution in a distributed manner.
  7. Debian has a stable branch that tests packages before release.
  8. It is known for being consistent and maintains a highly secure system.
  9. It supports almost every available Kernel maintained CPU instructions set.
  10. The installation is minimal, thus making it easier for server resources and their security.

## Disadvantages of Debian

  1. New software needs to be upgraded to get a stable repository. Still, sometimes it is difficulty to get the latest features and software updates as fast as it is available for other distributions.
  2. If you are an experienced person to work at the terminal end, then interacting with the system is easy. It gets a bit challenging for new users to get them working for the first time and is less user-friendly.
  3. It does not have an enterprise version like other distributions that offers you to work with large companies and their projects.
  4. Debian offers you an extended support cycle that even your hardware will probably get recycled before its support cycle ends.
  5. Though Debian works well with VMs, it still faces unexpected issues like sudden reboot, and server clock stuck, etc.

## What is CentOS?

  -> CentOs was released in 2004 and has been an open-source software. It is an enterprise-class Linux distribution supported by the red hat community. It is considered to be the replica of red hat enterprise Linux (RHEL) and is commonly used in IT world on a large scale.
  -> Being similar to RHEL, it allows you to develop in a more dominant and the best Linux distribution. CentOS is the **most popular** distribution when it comes to server environments.
  -> Due to RHEL support, CentOs ensures enterprise-level security, thus making it safe for users. It is highly customizable and stable.

## Features of CentOS

  1. It comes with many security in-built features that help protect from cyber-attacks using SELinux. It helps to reduce vulnerabilities of privilege escalation attacks.
  2. Many organizatons prefer it due to it extended support cycle.
  3. It uses the Yellowdog Update package manager that keeps your system up-to-date. This feature ensures that you can easily add or remove features from your application irrespective of your application phase.
  4. CentOS comes with a great and simple document that allows you to install and configure CentOS on your system efficiently.
  5. It can support multiple management platforms like cPanel, WebMin, Docker, etc.

## Advantages of CentOS

  1. CentOS is a complete workhouse with a stable distribution.
  2. You can ensure easy updates of the system and security with YUM.
  3. It allows you to install multiple PHP versions that are available for different users.
  4. As it has Red Hat backup, most of Red Hat's instructions work the same for CentOS, like a package manager.
  5. It comes with built-in management tools for containers.
  6. CentOS comes with RPM package compability that allows easy machine setup for development.
  7. It has a customized command line that ensures easy automation of new instance deployments.
  8. It has Docker compability.
  9. It can even provide high performance on the average hardware.
  10. It ensures easy and quick deployments.

## Disadvantages of CentOS

  1. 

## Diference between CentOS and Debian

-> CentOS vs Debian are two flavors of linux operating systems. CentOS is a linux distribution. It is free and open source. It is enterprise-claass-industries can use meaning for server building.

-> Debian is a Unix like computer operating system that is made up of open source components. It is built and supported by a group of individuals who are under the Debian project. Debian uses linux as its Kernel.

-> Debian has more up to date packages and because it is easier to upgrade to a newer version. 
