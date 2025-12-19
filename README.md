# Open Cognitive Kernel (OCK)

Open Cognitive Kernel (OCK) is an open-source, model-agnostic cognitive kernel that defines how AI systems are allowed to interact with data, memory, tools, time, and the real world in a safe, auditable, and bounded way.

OCK is **not a model**, **not an agent**, and **not a prompt framework**.
It is an architectural governance layer between AI models and real-world consequences.

---

## Why This Exists

Modern AI systems are increasingly capable, but their interaction with the world is governed by ad-hoc, proprietary, and opaque scaffolding. Models are often granted tool access, memory, and autonomy without a shared, inspectable, or principled control layer.

OCK exists to provide:
- Explicit permissioning instead of implicit trust
- Bounded authority instead of open-ended autonomy
- Auditable state instead of hidden behavior
- Model interchangeability instead of vendor lock-in

---

## Core Principles (Axioms)

1. Models are replaceable; architecture is not  
2. No cognition without context  
3. No action without permission  
4. No memory without ownership  
5. No authority without auditability  
6. No irreversible action without escalation  
7. No hidden state  
8. No silent failure  
9. The kernel does less, not more  
10. If it cannot be inspected, it cannot be trusted  

---

## What OCK Is

- A **governor**, not an intelligence
- A **kernel**, not a product
- A **contract** between models and reality
- A **shared safety substrate** for AI systems

---

## What OCK Is Not

- Not an autonomous agent
- Not an alignment philosophy
- Not a reasoning engine
- Not a replacement for models
- Not a commercial platform

---

## High-Level Architecture

OCK separates AI systems into three layers:

### 1. Kernel (Authoritative, Deterministic)
- Action type registry
- Permission and capability gating
- Memory ownership and scope
- Rate and cost limiting
- Full audit logging

### 2. Model (Non-Authoritative)
- Generates text and requests
- Proposes actions
- Has no direct access to tools, memory, or execution

### 3. Userland (Optional, Experimental)
- Agents, planners, personalities
- Domain-specific logic
- Runs entirely on top of the kernel

Only the kernel is allowed to affect the real world.

---

## Current Status

This project is in its earliest exploratory phase.
The initial focus is on:
- Defining a minimal action schema
- Implementing a reference verification loop
- Stress-testing permission and containment logic

This repository prioritizes **clarity and correctness over features**.

---

## License

MIT License
