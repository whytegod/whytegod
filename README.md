# Whytegod

**Whytegod** is an AI-first, peer-to-peer financial execution protocol specification built on top of the **Open Financial Network (OFN)**.

This repository defines a **standardized, intent-based execution layer** for financial actions, where users express *what they want to achieve* and compliant systems determine *how execution occurs*.

Whytegod is not an application.  
It is a protocol specification.

---

## Purpose

Modern financial systems require users to manually manage execution details:
- routing
- counterparties
- timing
- trust assumptions

Whytegod introduces an **intent-first abstraction** that separates:
- **User intent**
- **Execution logic**
- **Settlement and trust layers**

This enables AI-driven, policy-constrained execution while remaining compatible with open financial networks such as OFN.

---

## Core Concepts

### Intent-Based Execution
Users express goals (intents), not procedures.

The protocol defines:
- how intents are structured
- how they are validated
- how they flow through execution stages
- how failure modes are handled

### AI as an Execution Agent
AI systems may assist in:
- intent interpretation
- execution path selection
- optimization within defined constraints

AI does **not** replace protocol rules.  
All actions remain bounded by explicit specifications.

### Protocol Neutrality
Whytegod does not mandate:
- chains
- tokens
- custody models
- jurisdictions

It defines **interfaces**, not implementations.

---

## Repository Structure

This repository is organized as a protocol specification:

- `INTENT.md` — Intent model and abstraction
- `FLOW.md` — End-to-end execution flow
- `EXECUTION.md` — Execution mechanics and constraints
- `INTERFACE.md` — System interaction boundaries
- `schema/` — Machine-readable intent schemas
- `SECURITY.md` — Threat model and safeguards
- `ROLES.md` — Participant roles and responsibilities
- `governance/` — Governance boundaries and evolution
- `REFERENCE_IMPLEMENTATION.md` — Non-production reference logic
- `OFN_ALIGNMENT.md` — Alignment with OFN principles
- `OFN_STATUS.md` — Current OFN integration status
- `ROADMAP.md` — Planned evolution of the specification
- `CONTRIBUTING.md` — Contribution guidelines

---

## Design Principles

Whytegod is built on the following principles:

- Intent-first architecture
- Explicit execution boundaries
- Minimal trust assumptions
- Human-readable and machine-readable parity
- Compatibility with open financial networks
- Specification before implementation

Any extension or contribution must preserve these principles.

---

## Status

Whytegod is currently a **protocol specification**.

- No production deployment
- No live smart contracts
- No token
- No guarantees of execution

Implementation is intentionally deferred to allow:
- public review
- ecosystem alignment
- specification stability

---

## OFN Alignment

Whytegod is designed to operate **on top of** the Open Financial Network (OFN).

It does not modify OFN core protocols.  
It defines an execution abstraction that can be adopted by OFN-compliant systems.

Current alignment status is documented in `OFN_ALIGNMENT.md` and `OFN_STATUS.md`.

---

## Contributing

Contributions are welcome within defined scope.

Please read `CONTRIBUTING.md` before opening issues or pull requests.

This repository prioritizes:
- clarity
- correctness
- long-term protocol integrity

---

## License

This specification is provided for open review and discussion.

Licensing details will be finalized prior to any production implementation.