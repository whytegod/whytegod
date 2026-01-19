# WHYTGOD

Whytegod is an AI-first, peer-to-peer financial execution layer built on top of the Open Financial Network (OFN).

It is not a blockchain, not a wallet, and not a trading platform.

Whytegod is a **coordination and execution protocol** that translates user intent into validated, governed financial actions across OFN-compatible systems.

---

## What Whytegod Is

Whytegod defines **how financial intent is expressed, validated, and executed** in a decentralized environment.

It provides:
- A standard way to describe user intent
- A clear interface for execution systems
- A governed execution flow
- A reference path for real-world implementation

Whytegod does **not** custody funds, issue assets, or enforce financial outcomes.

---

## What Whytegod Is Not

- Not a bank  
- Not an exchange  
- Not a smart contract platform  
- Not an investment product  
- Not a custodial service  

Whytegod is strictly an **execution-layer protocol**.

---

## Core Concepts

### Intent
User actions are expressed as structured intents rather than direct commands.

See: `INTENT.md`

---

### Interface
Execution systems interact with Whytegod through a defined interface.

See: `INTERFACE.md`

---

### Validation
All intents must pass schema and rule validation before execution.

See: `schema/`

---

### Execution
Execution is deterministic, auditable, and non-custodial.

See: `EXECUTION.md`

---

### Flow
Whytegod defines a full lifecycle from intent creation to execution outcome.

See: `FLOW.md`

---

## Governance

Protocol rules, evolution, and safeguards are governed through explicit documentation.

See: `governance/`  
See also: `ROLES.md`

---

## Security Model

Whytegod prioritizes:
- Non-custodial execution
- Deterministic behavior
- Explicit failure handling
- Minimal trust assumptions

See: `SECURITY.md`

---

## OFN Relationship

Whytegod is designed to operate **on top of** the Open Financial Network (OFN).

- Whytegod does not modify OFN
- Whytegod does not claim OFN ownership
- Whytegod aligns with OFN execution principles

See:
- `OFN_ALIGNMENT.md`
- `OFN_STATUS.md`

---

## Reference Implementation

A minimal, non-prescriptive reference outline is provided to demonstrate implementability.

This reference does **not** define production behavior.

See: `REFERENCE_IMPLEMENTATION.md`

---

## Roadmap

Planned milestones and evolution are documented separately.

See: `ROADMAP.md`

---

## Status

This repository defines **Whytegod Protocol Specification v0.1**.

The protocol is:
- Specification-complete
- Open for review
- Open for implementation

---

## License

Open specification.  
Implementation details are intentionally left flexible.