# Azure Labs

A collection of hands-on Azure labs completed while preparing for the **Microsoft Certified: Azure Administrator Associate (AZ-104)** certification.

The purpose of this repository is to strengthen practical Azure administration skills by deploying, configuring, troubleshooting, and documenting real Azure services. Each lab includes architecture, implementation steps, screenshots, troubleshooting notes, and key lessons learned.

---

## Objectives

- Gain hands-on experience with Azure services
- Reinforce AZ-104 concepts through practical labs
- Develop troubleshooting and documentation skills
- Build a professional Azure portfolio for future cloud engineering roles

---

## Technologies

This repository will cover:

- Azure Resource Groups
- Azure Storage
- Azure Virtual Networks
- Network Security Groups (NSGs)
- Azure Bastion
- Virtual Machines
- Azure Backup
- Recovery Services Vault
- Azure RBAC
- Azure Policy
- Azure Monitor
- Azure Load Balancer
- Application Gateway
- Azure Key Vault
- Managed Identities
- VM Scale Sets
- Azure CLI
- PowerShell
- Bicep

---

# Lab Index

| Lab | Status | Description |
|------|:------:|-------------|
| [Lab 01 – Resource Groups](Lab-01-Resource-Groups/) | ✅ | Create Resource Groups, apply tags, move resources, and understand Resource Group organization. |
| [Lab 02 – Virtual Networks](Lab-02-Virtual-Networks/) | ✅ | Create VNets, configure address spaces, design subnets, and understand Azure networking fundamentals. |
| [Lab 03 – Linux Virtual Machine](Lab-03-Linux-Virtual-Machine/) | ✅ | Deploy a Linux VM, configure networking, connect via SSH, and explore VM components. |
| Lab 04 – Network Security Groups | 🚧 Planned | Secure VM traffic using inbound and outbound NSG rules and understand rule evaluation. |
| Lab 05 – Azure Bastion | 🚧 Planned | Securely administer Linux and Windows VMs without exposing RDP or SSH to the Internet. |
| Lab 06 – VNet Peering | 🚧 Planned | Connect two Virtual Networks, verify communication, and understand peering limitations. |
| Lab 07 – Storage Accounts | 🚧 Planned | Deploy Storage Accounts, configure redundancy, explore Blob Storage, Azure Files, and SAS tokens. |
| Lab 08 – Managed Disks & Snapshots | 🚧 Planned | Create managed disks, attach data disks, create snapshots, and compare snapshots with Azure Backup. |
| Lab 09 – Recovery Services Vault & Azure Backup | 🚧 Planned | Configure Azure Backup, create recovery points, and restore protected resources. |
| Lab 10 – Availability Sets & Availability Zones | 🚧 Planned | Deploy highly available VMs and understand fault domains, update domains, and zones. |
| Lab 11 – Azure Load Balancer | 🚧 Planned | Configure a Layer 4 Load Balancer, backend pools, health probes, and balancing rules. |
| Lab 12 – Azure Application Gateway | 🚧 Planned | Deploy an Application Gateway, configure listeners, routing rules, and optionally enable WAF. |
| Lab 13 – Azure RBAC | 🚧 Planned | Assign built-in roles, test permissions, and understand Azure authorization. |
| Lab 14 – Azure Policy & Resource Locks | 🚧 Planned | Enforce governance with Azure Policy and protect resources using locks. |
| Lab 15 – Azure Key Vault | 🚧 Planned | Store secrets, certificates, and keys, and manage secure access. |
| Lab 16 – Managed Identities | 🚧 Planned | Enable managed identities and securely access Azure resources without storing credentials. |
| Lab 17 – Azure Monitor & Alerts | 🚧 Planned | Configure monitoring, metrics, activity logs, Log Analytics, and alert rules. |
| Lab 18 – VM Scale Sets | 🚧 Planned | Deploy VM Scale Sets and configure autoscaling based on demand. |
| Lab 19 – Azure CLI & PowerShell Automation | 🚧 Planned | Deploy and manage Azure resources using Azure CLI and PowerShell. |
| Lab 20 – Bicep Infrastructure as Code | 🚧 Planned | Deploy Azure infrastructure using reusable Bicep templates. |
| *(More labs will be added as the repository grows.)* | | |

---

## Repository Structure

```text
azure-labs/
│
├── README.md
│
├── Lab-01-Resource-Groups/
│   ├── README.md
│   └── images/
│
├── Lab-02-Virtual-Networks/
│   ├── README.md
│   └── images/
│
├── Lab-03-Network-Security-Groups/
│   ├── README.md
│   └── images/
│
└── ...
```

---

## Learning Approach

Each lab follows a consistent documentation structure:

- Objective
- Architecture
- Lab Tasks
- Implementation Steps
- Verification
- Troubleshooting
- Lessons Learned
- Key Takeaways

---

## Certification Goal

This repository documents my hands-on Azure learning journey while preparing for the **Microsoft Certified: Azure Administrator Associate (AZ-104)** certification and serves as a portfolio of practical cloud administration experience.
