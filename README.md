# Azure Security SOC Lab

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?logo=microsoftazure&logoColor=white)
![SOC](https://img.shields.io/badge/SOC-Lab-success)
![Cloud Security](https://img.shields.io/badge/Cloud-Security-blue)
![Microsoft Sentinel](https://img.shields.io/badge/Microsoft-Sentinel-5C2D91)

---

## Overview

This repository documents my Azure Security SOC Lab built using a Microsoft Azure Trial subscription.

The objective of this project was to build an enterprise-style Azure infrastructure that could later integrate with Microsoft Sentinel, Microsoft Defender XDR, Azure Arc, and Log Analytics Workspace while learning Azure cloud security fundamentals.

Although the Azure trial has expired, this repository preserves the deployment process, screenshots, architecture, configuration steps, and lessons learned throughout the lab.

---

# Project Objectives

- Build Azure infrastructure from scratch
- Learn Azure networking
- Deploy Windows Virtual Machines
- Configure Azure Storage
- Prepare Azure environment for Microsoft Sentinel
- Understand Azure security services
- Learn Azure Monitor and Log Analytics
- Build a foundation for Microsoft Security Operations

---

# Technologies Used

- Microsoft Azure
- Azure Resource Groups
- Azure Virtual Networks
- Azure Virtual Machines
- Azure Storage Accounts
- Azure Monitor
- Log Analytics Workspace
- Azure Arc
- Microsoft Sentinel
- Windows 10
- Windows Server

---

# Azure Services Implemented

- Resource Groups
- Virtual Networks
- Address Spaces
- Subnets
- Windows Virtual Machines
- Azure Storage Account
- Azure Monitor
- Log Analytics Workspace

---

# Deployment Workflow

## 1. Create Resource Group

Created a Resource Group to logically organize all Azure resources.

Purpose:

- Centralized resource management
- Easy deployment
- Cost management
- Easy cleanup

---

## 2. Create Virtual Network

Configured a dedicated Azure Virtual Network.

Implemented:

- Private Address Space
- Multiple Subnets
- Network Segmentation

---

## 3. Configure Subnets

Created multiple subnets including:

- Application Subnet
- Database Subnet
- Management Subnet

to simulate enterprise infrastructure.

---

## 4. Deploy Windows Virtual Machine

Created Windows Virtual Machines using Azure Marketplace.

Configured:

- Windows 10
- Standard SSD
- Public IP
- RDP Access
- Azure Networking

---

## 5. Create Storage Account

Configured Azure Storage Account using:

- Standard Performance
- LRS Redundancy
- Blob Storage

---

## 6. Azure Monitor

Configured Azure Monitor to collect infrastructure telemetry.

Used for:

- Resource Monitoring
- Performance Monitoring
- Log Collection

---

## 7. Log Analytics Workspace

Prepared Log Analytics Workspace for centralized log collection and future Microsoft Sentinel integration.

---

# Skills Demonstrated

- Azure Administration
- Azure Networking
- Cloud Infrastructure
- Virtual Machines
- Storage
- Azure Monitor
- Log Analytics
- Cloud Security
- Microsoft Sentinel Preparation

---

# Repository Contents

```
Azure-Security-SOC-Lab

README.md

AZURE INFRASTRUCTURE SETUP.docx

AZURE-CLOUD.docx
```

---

# Lessons Learned

- Azure Resource Management
- Azure Networking
- Virtual Machine Deployment
- Cloud Monitoring
- Storage Configuration
- Azure Security Fundamentals

---

# Future Improvements

- Azure Firewall
- Azure Bastion
- Azure Key Vault
- Microsoft Defender for Cloud
- Azure Arc
- Microsoft Sentinel Analytics Rules
- Azure Automation
- Defender XDR Integration

---

# Project Status

**Status:** Completed

**Environment:** Microsoft Azure Trial

**Current State:** Decommissioned (Azure Trial Expired)

---

## Author

**Badavula Kumar Teja**

SOC Analyst | Microsoft Sentinel | Microsoft Defender XDR | Azure Security | Qualys VMDR
