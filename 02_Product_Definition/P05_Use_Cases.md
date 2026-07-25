# Use Cases

Document ID: P05

Project: Trafico

Version: 1.0

Status: Draft

Last Updated: July 2026

---

# 1. Purpose

This document defines the primary interactions between users and the Trafico platform. Each use case describes how users achieve a specific goal using the system.

---

# 2. Actors

The following actors interact with the system:

- Business Owner
- Operator
- Customer
- Supplier
- System Administrator

---

# UC-001 Register Company

## Primary Actor

Business Owner

## Goal

Create a company account.

## Preconditions

- User is not registered.

## Main Flow

1. Open registration page.
2. Enter company information.
3. Verify email.
4. Create account.
5. Access dashboard.

## Postconditions

Company account created successfully.

---

# UC-002 Connect WhatsApp

## Primary Actor

Business Owner

## Goal

Connect WhatsApp Business Account.

## Main Flow

1. Open Settings.
2. Start Meta authorization.
3. Complete verification.
4. Save connection.

## Result

Business can receive WhatsApp messages.

---

# UC-003 Receive Customer Message

## Primary Actor

Customer

## Goal

Send a service request.

## Main Flow

1. Customer sends WhatsApp message.
2. Trafico receives webhook.
3. Conversation is created.
4. Operator is notified.

---

# UC-004 Assign Supplier

## Primary Actor

Operator

## Goal

Assign a supplier to a conversation.

## Main Flow

1. Open conversation.
2. Select supplier.
3. Save assignment.
4. Supplier receives request.

---

# UC-005 Relay Messages

## Primary Actor

System

## Goal

Securely relay messages.

## Main Flow

1. Receive message.
2. Validate message.
3. Run leak detection.
4. Store message.
5. Forward message.
6. Update conversation.

---

# UC-006 Detect Contact Sharing

## Primary Actor

System

## Goal

Prevent participants from sharing contact information.

## Main Flow

1. Receive message.
2. Analyze content.
3. Detect prohibited information.
4. Block message.
5. Notify operator.

---

# UC-007 Close Conversation

## Primary Actor

Operator

## Goal

Mark conversation as completed.

## Main Flow

1. Open conversation.
2. Review status.
3. Close conversation.
4. Archive history.

---

# 3. Summary

These use cases define the expected behavior of Trafico from the perspective of users and system interactions.