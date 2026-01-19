# WHYTEGOD

Whytegod is an **AI-first, intent-driven financial execution protocol** built on top of the **Open Financial Network (OFN)**.

It defines how user intent is expressed, validated, and executed across a decentralized financial system.

---

## What This Repository Is

This repository contains the **protocol specification** for Whytegod.

It is:
- A **design and specification layer**
- A **reference for builders, auditors, and integrators**
- A **foundation for future implementations**

It is **not**:
- A frontend application
- A deployed smart contract
- A custodial service

---

## Core Concept

Whytegod introduces **Intent-Based Finance**.

Instead of users interacting directly with complex financial systems, they express **intent**, and the protocol defines how that intent is safely interpreted and executed.

Example intent:
- “Swap token A for token B at the best available rate”
- “Move funds only if security conditions are met”

---

## Repository Structure

The repository is organized as follows:

- `INTENT.md` — Defines the intent model and structure  
- `schema/` — Machine-readable schemas for intent validation  
- `FLOW.md` — Describes how intents move through the system  
- `EXECUTION.md` — Defines execution rules and constraints  
- `INTERFACE.md` — Interface boundaries between system actors  
- `SECURITY.md` — Threat model and safety assumptions  
- `ROLES.md` — Roles within the protocol  
- `governance/` — Governance principles and controls  
- `OFN_ALIGNMENT.md` — Alignment with Open Financial Network principles  
- `OFN_STATUS.md` — Current status of OFN alignment  

---

## Start Here (Reading Order)

If you are new to Whytegod, read in this order:

1. [`INTENT.md`](./INTENT.md)  
2. [`FLOW.md`](./FLOW.md)  
3. [`EXECUTION.md`](./EXECUTION.md)  
4. [`INTERFACE.md`](./INTERFACE.md)  
5. [`schema/`](./schema)  
6. [`SECURITY.md`](./SECURITY.md)  

---

## Open Financial Network (OFN)

Whytegod is designed to operate within the principles of the **Open Financial Network (OFN)**.

The protocol emphasizes:
- Openness
- Interoperability
- Non-custodial execution
- User intent sovereignty

This repository **does not claim official OFN endorsement**.  
Alignment details are documented transparently.

---

## Project Status

Whytegod is currently in the **specification and design phase**.

- No production deployment
- No token issuance
- No live financial operations

All changes are experimental and subject to revision.

---

## License

MIT License