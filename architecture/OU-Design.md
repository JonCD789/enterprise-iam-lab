# Organizational Unit Design

## Domain

northwind.corp

## OU Structure

Northwind.corp

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

## Design Decisions

- Users are organized by department.
- Access will be assigned using Role-Based Access Control (RBAC).
- Computer objects are separated from user objects.
- Administrative accounts are isolated from standard user accounts.
- Disabled accounts are retained for audit and recovery purposes.
