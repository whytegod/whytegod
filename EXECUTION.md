# WHYTGOD Execution Flow

This document defines how WHYTGOD coordinates peer-to-peer financial execution
without custody of funds.

---

## 1. Core Role

WHYTGOD acts as an execution coordinator.

It:
- Receives execution intent
- Validates participants and constraints
- Routes execution through OFN-compatible rails
- Confirms finality

It does NOT:
- Hold user funds
- Act as a counterparty
- Guarantee profit or outcome

---

## 2. Execution Participants

Each execution involves:

1. Initiator
   - Requests an action (send, swap, settle, route)

2. Counterparty (optional)
   - Another peer or system endpoint

3. WHYTGOD
   - Validates, coordinates, and enforces rules

4. OFN Rail
   - Executes the actual financial movement

---

## 3. Execution Lifecycle

### Step 1 — Intent Submission
A user submits an execution intent specifying:
- Action type
- Asset
- Amount
- Conditions (if any)

---

### Step 2 — Validation
WHYTGOD validates:
- Structural correctness
- Risk boundaries
- Governance rules
- Security constraints

Invalid intents are rejected.

---

### Step 3 — Routing
Valid intents are routed to:
- Appropriate OFN-compatible rails
- Approved execution paths only

---

### Step 4 — Execution
Funds move directly between peers or endpoints.
WHYTGOD never holds custody.

---

### Step 5 — Confirmation
WHYTGOD records execution status:
- Success
- Failure
- Partial (if allowed)

---

## 4. Trust Model

WHYTGOD enforces trust through:
- Deterministic rules
- Transparent validation
- Minimal discretionary control

Users retain full control of assets at all times.

---

## 5. Failure Handling

If execution fails:
- Funds remain with original owner
- No forced retries
- Clear error signaling

---

## 6. Design Principle

Execution clarity > speed  
Safety > features  
Coordination > custody
