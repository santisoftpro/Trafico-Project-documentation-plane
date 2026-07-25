# Business Rules

Document ID: P08

Project: Trafico

Version: 1.0

Status: Draft


Last Updated: July 2026

---

# 1. Purpose

This document defines the business rules that govern how Trafico operates. Business rules ensure the platform behaves consistently regardless of the underlying technology or implementation.

---

# 2. Company Rules

BR-001

Each company must have exactly one owner.

---

BR-002

A company subscription must be active before the company can use messaging services.

---

BR-003

Each company operates independently.

No company can access another company's data.

---

# 3. User Rules

BR-004

Every user belongs to exactly one company.

---

BR-005

Every user must have an assigned role.

---

BR-006

Inactive users cannot access the platform.

---

# 4. Customer Rules

BR-007

Customers may have multiple conversations.

---

BR-008

Customer contact information is only visible to authorized users.

---

# 5. Supplier Rules

BR-009

Suppliers may serve multiple companies if permitted.

---

BR-010

Suppliers cannot directly access customer information unless explicitly allowed.

---

# 6. Conversation Rules

BR-011

Every conversation belongs to one company.

---

BR-012

Every conversation must have a status.

Possible statuses include:

- New
- Assigned
- In Progress
- Waiting
- Completed
- Archived

---

BR-013

Completed conversations become read-only.

---

# 7. Messaging Rules

BR-014

Every message belongs to exactly one conversation.

---

BR-015

Messages cannot be permanently deleted by operators.

---

BR-016

Every forwarded message must be stored.

---

# 8. Leak Detection Rules

BR-017

Messages containing prohibited contact information shall be flagged.

---

BR-018

Blocked messages shall not be forwarded.

---

BR-019

Every leak attempt shall be logged.

---

# 9. Security Rules

BR-020

Users may only access company data they own.

---

BR-021

All sensitive actions shall be recorded in the audit log.

---

# 10. Summary

Business rules define the operational policies that every module of Trafico must follow regardless of implementation.