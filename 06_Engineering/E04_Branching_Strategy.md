# Branching Strategy

Document ID: E04

Project: Trafico

Version: 1.0

Status: Draft

Last Updated: July 2026

---

# 1. Purpose

Defines how branches are created, maintained, and merged.

---

# 2. Branch Types

main

develop

feature/*

bugfix/*

release/*

hotfix/*

---

# 3. Merge Policy

Feature

↓

Develop

↓

Release

↓

Main

---

# 4. Protection Rules

Protect main.

Require reviews.

Require passing CI.

No direct pushes.

---

# 5. Summary

Branch management should minimize conflicts and protect production stability.