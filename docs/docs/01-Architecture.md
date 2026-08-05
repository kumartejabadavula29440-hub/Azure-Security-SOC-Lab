# Azure Security SOC Lab Architecture

## Overview

This document describes the overall architecture of the Azure Security SOC Lab that I built using a Microsoft Azure Trial subscription.

The purpose of this lab was to understand Azure cloud infrastructure deployment and prepare a secure environment for Microsoft security services such as Microsoft Sentinel, Azure Monitor, Azure Arc, and Log Analytics Workspace.

Although the environment has been decommissioned after the Azure trial expired, this documentation captures the architecture, deployment approach, and security considerations implemented during the project.

---

# Lab Objectives

The architecture was designed to achieve the following objectives:

- Learn Azure cloud infrastructure deployment
- Understand Azure networking concepts
- Deploy enterprise-style virtual machines
- Implement logical network segmentation
- Prepare infrastructure for Microsoft Sentinel integration
- Configure centralized monitoring using Azure Monitor
- Build a practical cloud security lab for SOC operations

---

# High-Level Architecture

```
                    Microsoft Azure Subscription
                               │
                               ▼
                      Resource Group
                               │
                               ▼
                     Virtual Network (VNet)
                               │
        ┌──────────────┬──────────────┬──────────────┐
        │              │              │
   App Subnet     Database Subnet   Management Subnet
        │              │              │
        └──────────────┴──────────────┘
                       │
                Windows Virtual Machines
                       │
                Azure Monitor Agent
                       │
                       ▼
           Log Analytics Workspace
                       │
                       ▼
              Microsoft Sentinel
```

---

# Azure Components

## Resource Group

The Resource Group was used as the logical container for all Azure resources created during the project.

Benefits:

- Centralized resource management
- Simplified deployment
- Easier resource cleanup
- Better organization
- Cost management

---

## Virtual Network

A dedicated Virtual Network (VNet) was created to provide network isolation for all deployed resources.

The VNet provided:

- Private address space
- Secure communication
- Resource isolation
- Foundation for subnet segmentation

---

## Network Segmentation

The virtual network was divided into multiple subnets to simulate an enterprise deployment.

The environment included:

- Application Subnet
- Database Subnet
- Management Subnet

This separation improves security by reducing unnecessary communication between workloads.

---

## Virtual Machines

Windows Virtual Machines were deployed to simulate enterprise endpoints and infrastructure.

Configuration included:

- Windows operating system
- Standard SSD storage
- Administrator account
- Remote Desktop (RDP) access
- Azure virtual networking

These systems later became candidates for monitoring and security onboarding.

---

## Azure Storage

Azure Storage Accounts were created for cloud-based storage requirements.

Configuration:

- Standard Performance
- Locally Redundant Storage (LRS)
- Blob Storage

---

## Azure Monitor

Azure Monitor was implemented to collect infrastructure telemetry and monitor resource health.

Collected information includes:

- Performance metrics
- Resource health
- Diagnostic logs
- Monitoring data

---

## Log Analytics Workspace

Log Analytics Workspace serves as the centralized repository for Azure monitoring data.

Its responsibilities include:

- Collecting logs from Azure resources
- Supporting Azure Monitor
- Providing KQL-based log analysis
- Serving as the backend for Microsoft Sentinel

---

## Microsoft Sentinel Integration

The environment was designed to support Microsoft Sentinel.

After Log Analytics Workspace was configured, Microsoft Sentinel could be enabled to provide:

- Centralized security monitoring
- Security analytics
- Incident management
- Threat detection
- Investigation workflows

---

# Security Considerations

During the architecture design, the following security principles were considered:

- Resource isolation
- Network segmentation
- Controlled administrative access
- Centralized monitoring
- Logging
- Cloud security best practices

---

# Skills Demonstrated

This project demonstrates practical knowledge of:

- Microsoft Azure
- Azure Networking
- Virtual Machines
- Resource Groups
- Azure Storage
- Azure Monitor
- Log Analytics Workspace
- Microsoft Sentinel preparation
- Cloud Security Architecture

---

# Lessons Learned

During this project, I gained practical experience in:

- Designing Azure infrastructure
- Building secure virtual networks
- Deploying Windows virtual machines
- Organizing Azure resources
- Preparing cloud infrastructure for Microsoft security services
- Understanding enterprise cloud architecture

---

# Future Enhancements

If the environment is rebuilt, the following services will be integrated:

- Microsoft Defender for Cloud
- Azure Firewall
- Azure Bastion
- Azure Key Vault
- Azure Load Balancer
- Azure Application Gateway
- Azure Arc
- Microsoft Defender XDR
- Microsoft Sentinel Analytics Rules

---

## Summary

This architecture provides a practical foundation for learning Azure infrastructure, cloud networking, monitoring, and Microsoft security technologies while simulating an enterprise Security Operations Center (SOC) environment.
