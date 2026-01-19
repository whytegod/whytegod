# Whytegod Interface Specification

## Purpose

This document defines the external and internal interfaces of the Whytegod protocol.

The interface layer describes **how actors interact with the system**, not how execution is implemented internally.  
Its goal is to provide a **stable, minimal, and deterministic contract** between users, agents, and execution infrastructure.

This file is intentionally implementation-agnostic.

---

## Interface Principles

The Whytegod interface follows these rules:

- Interfaces are **explicit and narrow**
- All actions originate from **declared intent**
- Interfaces do not contain business logic
- Interfaces do not imply custody
- Interfaces must be deterministic and verifiable
- Interfaces must be safe to expose publicly

---

## Interface Actors

The protocol defines the following interface actors:

### 1. User

A User is an external actor that expresses intent.

Capabilities:
- Create intent objects
- Submit intent for processing
- Query intent status
- Verify execution results

Limitations:
- Cannot execute actions directly
- Cannot mutate execution state
- Cannot bypass validation

---

### 2. Agent

An Agent is an optional intermediary that assists in intent formation or routing.

Capabilities:
- Assist users in constructing valid intent
- Submit intent on behalf of users (with permission)
- Monitor execution outcomes

Limitations:
- Cannot alter intent after submission
- Cannot force execution
- Cannot override validation rules

---

### 3. Interface Gateway

The Interface Gateway is the protocol-facing surface that receives intent.

Capabilities:
- Accept intent submissions
- Perform schema validation
- Reject invalid or malformed intent
- Forward validated intent to execution

Limitations:
- Does not execute financial actions
- Does not interpret intent meaning
- Does not store funds or assets

---

### 4. Execution Layer (Boundary)

The Execution Layer is **outside** the interface boundary.

The interface:
- Sends validated intent to execution
- Receives execution results
- Exposes results in a read-only manner

The interface does **not**:
- Control execution logic
- Guarantee execution success
- Modify execution outcomes

---

## Interface Objects

### Intent Object

The primary interface object is the **Intent**.

An intent:
- Is a structured declaration of desired outcome
- Is immutable once accepted
- Must conform to the published schema
- Is uniquely identifiable
- Is verifiable by third parties

The interface does not interpret intent semantics.

---

### Execution Result

An execution result represents the outcome of intent processing.

Properties:
- Linked to a single intent
- Deterministic and replay-safe
- Read-only once published
- May represent success, failure, or partial completion

---

## Interface Operations

### Submit Intent

Description:
- Accepts a structured intent object
- Validates against schema
- Either accepts or rejects atomically

Outcome:
- Accepted intent receives a unique identifier
- Rejected intent returns validation errors

---

### Query Intent Status

Description:
- Retrieves the current state of an intent
- Does not mutate protocol state

Possible states:
- Pending
- Executed
- Failed
- Rejected

---

### Retrieve Execution Result

Description:
- Returns the final execution outcome
- Read-only
- Verifiable

---

## Error Handling

Interface errors are explicit and non-destructive.

Error categories:
- Schema validation error
- Authorization error
- Interface availability error

The interface never:
- Silently fails
- Retries execution
- Alters intent content

---

## Security Boundaries

The interface layer enforces:

- Strict schema validation
- Immutable intent acceptance
- No custody of user assets
- No privileged execution access

Security guarantees stop at the interface boundary.

---

## Versioning

Interface changes:
- Are explicit
- Are backward-compatible where possible
- Never silently alter behavior

Breaking changes require a new interface version.

---

## Non-Goals

The interface does NOT:

- Act as a wallet
- Execute trades
- Guarantee liquidity
- Provide financial advice
- Replace OFN components

---

## Summary

The Whytegod interface exists to:

- Safely accept intent
- Clearly separate responsibility
- Provide deterministic interaction
- Remain simple, stable, and inspectable

All complexity lives **outside** the interface.