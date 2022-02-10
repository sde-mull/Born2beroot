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
