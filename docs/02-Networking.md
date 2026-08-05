# Azure Networking

## Overview

Networking is one of the most important components of any Azure environment. In this lab, a dedicated Azure Virtual Network (VNet) was created to provide secure communication between deployed resources while maintaining logical separation between workloads.

The objective was to simulate a simple enterprise network that could later support Microsoft Sentinel, Azure Monitor, and additional Microsoft security services.

---

# Objectives

The networking design was created to:

- Isolate Azure resources
- Organize workloads into logical network segments
- Prepare infrastructure for future security services
- Understand Azure Virtual Network concepts
- Learn subnet planning and IP addressing

---

# Virtual Network

A dedicated Virtual Network (VNet) was created for the lab environment.

The Virtual Network provides:

- Private communication between Azure resources
- Network isolation
- Secure resource connectivity
- Foundation for subnet segmentation

---

# Address Space

The Virtual Network was configured using a private IPv4 address range.

Benefits include:

- Organized IP allocation
- Simplified subnet management
- Reduced address conflicts
- Scalable network design

---

# Subnet Design

To simulate an enterprise environment, the VNet was divided into multiple subnets.

## Application Subnet

Purpose:

- Host application servers
- Separate application workloads from other resources

---

## Database Subnet

Purpose:

- Reserve dedicated network space for database workloads
- Improve logical separation

---

## Management Subnet

Purpose:

- Administrative resources
- Infrastructure management
- Future expansion for management services

---

# Network Segmentation

Network segmentation improves security by separating different workloads into individual network boundaries.

Advantages include:

- Reduced attack surface
- Easier traffic management
- Better resource organization
- Improved security

---

# Virtual Machine Connectivity

Windows Virtual Machines were deployed inside the Virtual Network.

Each VM received:

- Virtual Network interface
- Private IP address
- Network Security Group protection
- Remote Desktop access for administration

---

# Security Considerations

The following security concepts were considered during deployment:

- Private IP addressing
- Resource isolation
- Controlled RDP access
- Logical network segmentation
- Azure networking best practices

---

# Skills Demonstrated

- Azure Virtual Network
- Azure Subnets
- IP Address Planning
- Azure Networking
- Windows VM Networking
- Cloud Infrastructure Design

---

# Lessons Learned

Through this exercise, I gained hands-on experience with:

- Designing Azure Virtual Networks
- Creating subnets
- Planning IP address space
- Understanding network isolation
- Preparing cloud infrastructure for enterprise deployments

---

# Future Improvements

Future versions of the lab will include:

- Azure Firewall
- Azure Bastion
- Network Security Groups (Advanced Rules)
- Route Tables
- Private Endpoints
- VPN Gateway
- Azure Load Balancer

---

## Summary

The networking architecture provides a secure and scalable foundation for deploying Azure resources while preparing the environment for Microsoft security technologies and enterprise SOC operations.
