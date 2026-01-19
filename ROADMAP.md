# Whytegod Roadmap

This roadmap defines the phased development of Whytegod as an AI-first,
intent-based peer-to-peer (P2P) financial execution layer built on the
Open Financial Network (OFN).

The goal is clarity, not speed.

---

## Phase 1 — P2P MVP (Current Focus)

The first phase delivers a minimal, functional P2P execution system that
proves the core intent → execution flow.

### Objectives
- Enable peer-to-peer financial actions using intent-based abstraction
- Separate *what users want* from *how execution happens*
- Maintain OFN alignment without protocol coupling

### Scope
- User intent submission (buy, sell, send, receive)
- Intent validation and normalization
- Counterparty matching (manual or assisted)
- Execution state tracking (pending, in-progress, completed)
- Human-readable execution logs

### Explicitly Out of Scope
- Smart contracts
- Tokens or on-chain settlement
- Automated liquidity pools
- Regulatory enforcement
- Custodial asset holding

This phase is designed for learning, iteration, and clarity.

---

## Phase 2 — Assisted Execution & Interfaces

Once the P2P MVP is validated, the focus shifts to usability and assisted
execution.

### Objectives
- Introduce structured interfaces for intent creation
- Enable AI-assisted execution routing
- Improve observability and feedback loops

### Scope
- Basic web interface for P2P actions
- Execution suggestions and guardrails
- Error handling and retry flows
- Interface specification stabilization

---

## Phase 3 — Protocol Hardening & Ecosystem Alignment

This phase prepares Whytegod for external collaboration and long-term
protocol development.

### Objectives
- Harden specifications
- Improve interoperability
- Enable external contributors

### Scope
- Formalized schemas
- Governance process refinement
- Contributor onboarding documentation
- Extended OFN compatibility

---

## Guiding Principles

- Specification before implementation
- Human readability over abstraction
- Execution clarity over automation
- Minimal surface area at every phase

---

## Status

Whytegod is currently in **Phase 1 — P2P MVP**.