# Database Design

Document ID: A05

Project: Trafico

Version: 1.0

Status: Draft


Last Updated: July 2026

---

# 1. Purpose

This document defines the logical database design for the Trafico platform.

It identifies the primary entities, relationships, constraints, and database design principles required to support the application's business requirements.

---

# 2. Database Goals

The database should:

- Maintain data integrity.
- Support multi-tenancy.
- Scale efficiently.
- Prevent data duplication.
- Support auditing.
- Ensure high performance.

---

# 3. Primary Entities

The platform contains the following core entities:

- Company
- User
- Role
- Customer
- Supplier
- Conversation
- Participant
- Message
- Attachment
- Notification
- Subscription
- AuditLog
- LeakAttempt

---

# 4. Relationship Overview

Company

↓

Users

↓

Conversations

↓

Messages

↓

Attachments

Company

↓

Customers

↓

Conversations

Company

↓

Suppliers

↓

Conversations

---

# 5. Data Integrity Rules

- Every company owns its data.
- Every message belongs to one conversation.
- Every conversation belongs to one company.
- Foreign key constraints must be enforced.
- Soft deletes should be used where appropriate.

---

# 6. Indexing Strategy

Indexes should exist for:

- Conversation ID
- Customer ID
- Supplier ID
- Company ID
- Created Date
- Status

---

# 7. Audit Strategy

Critical operations shall be logged.

Examples include:

- Login
- Role changes
- Conversation assignment
- Subscription changes
- Security events

---

# 8. Summary

The Trafico database is designed using relational principles to ensure consistency, scalability, and maintainability.