# Organizational Unit (OU) Design

## Project

Enterprise Identity and Access Management Lab

---

## Purpose

This document defines the Organizational Unit (OU) structure for Northwind Health Systems.

The OU design provides a scalable and secure structure for managing users, computers, service accounts, and administrative objects while supporting Group Policy, delegation, and Role-Based Access Control (RBAC).

---

## Domain

northwind.corp

---

# Organizational Unit Structure

```text
northwind.corp

│

├── Admin Accounts

├── Service Accounts

├── Groups

├── Computers

├── Servers

├── Users

│   ├── Executive

│   ├── Information Technology

│   ├── Human Resources

│   ├── Finance

│   ├── Information Security

│   ├── Marketing

│   ├── Operations

│   ├── Nursing

│   ├── Clinical

│   ├── Facilities

│   └── Help Desk

├── Disabled Users

└── Contractors
```

---

# Design Decisions

- Users are organized by department rather than physical location.
- Security permissions will be assigned using Role-Based Access Control (RBAC).
- Administrative accounts are separated from standard user accounts.
- Disabled accounts are retained for audit and recovery purposes.
- Computers and servers are managed separately to simplify Group Policy administration.

---

# Future Work

Future phases will include:

- Security Group Design
- RBAC Design
- Group Policy Design
- Identity Lifecycle Management
- Microsoft Entra ID Synchronization
