# Domain Model

Document ID: A04

Project: Trafico

Version: 1.0

Status: Draft


Last Updated: July 2026

---

# 1. Purpose

This document defines the core business entities within Trafico and their relationships.

The domain model represents the business itself rather than the database implementation.

---

# 2. Core Domains

The Trafico platform is composed of the following domains:

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
- Audit Log
- Leak Attempt

---

# 3. Domain Responsibilities

## Company

Represents a business using Trafico.

---

## User

Represents employees of a company.

---

## Customer

Represents the client requesting services.

---

## Supplier

Represents the service provider.

---

## Conversation

Represents a communication session.

---

## Message

Represents an exchanged message.

---

## Attachment

Represents files attached to messages.

---

## Notification

Represents system-generated alerts.

---

## Subscription

Represents the company's billing plan.

---

## Audit Log

Records security-sensitive events.

---

## Leak Attempt

Records blocked attempts to share restricted contact information.

---

# 4. Domain Relationships

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

Company

↓

Suppliers

---

# 5. Summary

The domain model provides a shared understanding of the business concepts that form the foundation of the Trafico platform.