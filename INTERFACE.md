# WHYTGOD Execution Interface

## 1. Purpose

The WHYTGOD Execution Interface defines the **only public interaction surface** of the protocol.

WHYTGOD does not custody funds, provide guarantees, or make decisions on behalf of users.  
It **receives execution intents**, validates them, routes them through supported Open Financial Network (OFN) rails, and returns execution results.

This interface is **deterministic, minimal, and non-custodial by design**.

---

## 2. Accepted Execution Intents

WHYTGOD accepts the following intent categories:

- Peer-to-peer asset exchange intents  
- Payment routing intents  
- Liquidity discovery intents  
- Settlement coordination intents  

Each intent represents a **request to execute**, not a promise of outcome.

WHYTGOD does not originate intents.  
All intents are externally generated.

---

## 3. Required Intent Fields

Every execution intent MUST include:

- `intent_id` — unique identifier
- `intent_type` — category of execution
- `asset_in` — asset being provided
- `asset_out` — asset being requested
- `amount` — execution quantity
- `counterparty_constraints` — execution limits or conditions
- `network_context` — OFN-compatible routing metadata
- `timestamp` — intent creation time

Intents missing required fields are **rejected without processing**.

---

## 4. Validation Guarantees

WHYTGOD guarantees that:

- Intents are syntactically validated before execution
- Execution rules are applied consistently
- No hidden state is introduced
- No asset custody occurs at any stage
- Execution paths are deterministic given identical inputs

WHYTGOD does **not** alter user-defined constraints.

---

## 5. Explicit Non-Guarantees

WHYTGOD does NOT guarantee:

- Execution success
- Price stability
- Counterparty behavior
- Network availability
- Liquidity presence
- Regulatory outcomes

WHYTGOD is an **execution layer**, not a financial advisor, broker, or custodian.

---

## 6. Versioning Rule

The execution interface follows **strict versioning**.

- Breaking changes require a new major version
- Deprecated fields remain readable but non-functional
- Historical intents remain verifiable

Once published, an interface version is **never retroactively altered**.

---

## 7. Interface Stability Statement

This interface is intentionally narrow.

Expansion occurs only through:
- New intent types
- New validation rules
- New routing contexts

Core principles remain immutable.
