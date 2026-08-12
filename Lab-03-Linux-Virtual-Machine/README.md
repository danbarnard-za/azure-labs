# Lab 03 – Linux Virtual Machine

## 🎯 Objective

Deploy and configure a Linux Virtual Machine in Azure, understand the resources that support the VM, connect securely using SSH, and explore VM lifecycle, networking, resizing, and resource dependencies.

---

## Prerequisites

- Azure Subscription
- Azure Portal
- Existing Virtual Network from Lab 02
- Azure Cloud Shell
- SSH key pair

---

## Technologies

- Azure Virtual Machines
- Linux / Ubuntu
- Azure Virtual Network
- Azure Subnets
- Network Interface (NIC)
- Public IP Address
- Network Security Group (NSG)
- Managed Disks
- SSH
- Azure Cloud Shell

---

## Lab Tasks

- [x] Deploy a Linux Virtual Machine
- [x] Configure the VM to use the existing VNet
- [x] Place the VM in the Frontend subnet
- [x] Configure SSH key authentication
- [x] Connect to the VM using SSH
- [x] Explore the VM's supporting resources
- [x] Test VM stop and deallocation behavior
- [x] Resize the VM
- [x] Test resource dependencies
- [x] Delete the VM and inspect remaining resources

---

## Architecture

```text
Subscription
│
└── RG-Networking
      │
      ├── VNet-Production
      │      │
      │      └── Frontend (10.0.1.0/24)
      │               │
      │               └── LinuxVM01
      │                      │
      │                      ├── Network Interface
      │                      ├── Private IP
      │                      ├── Public IP
      │                      ├── Network Security Group
      │                      ├── Managed OS Disk
      │                      └── SSH Key
      │
      └── Other subnets from Lab 02
