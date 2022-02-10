# Concepts

## How a virtual machine works?

-> Virtual machines are made possible through virtualization technology. Virtualization uses software to simulate virtual hardware that allows multiple VMs to run in a single machine. Thephysical machine is known as the host while the VMs running on it are called guests.

-> This process is managed by software known as hypervisor. The hypervisor is responsible for managing and provising resources (like memory and storage) from the host to guest. It also schedules operations in VMs so they don't overrun each other when using resources.

-> There are two types of hypervisors used in virtualization:
   1. Type 1 hypervisors are installed natively on the underlying physical hardware. VMs interact directly with hosts to allocate hardware resources without any           extra software layers in between. Host machines running type 1 hypervisors are used only for virtualization. They're often found in server based enviroments         like enterprise datacenters. A seperate management tool is needed to handle guest activities like creating new virtual machine instances or managing                 permissions.
