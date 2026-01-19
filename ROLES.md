# Execution Roles

Whytegod operates as an intent-driven execution network composed of distinct roles.

## 1. Requester
The entity that submits an execution intent.

Responsibilities:
- Define intent parameters
- Specify constraints
- Sign intent (off-chain or on-chain)

## 2. Solver
A solver interprets intents and proposes execution paths.

Responsibilities:
- Optimize execution route
- Respect intent constraints
- Submit execution proposals

## 3. Matcher
The matcher evaluates solver proposals.

Responsibilities:
- Compare multiple solver outputs
- Select optimal execution
- Prevent constraint violations

## 4. Validator
Validators verify correctness and integrity.

Responsibilities:
- Validate schema compliance
- Enforce execution rules
- Reject invalid or malicious intents

## 5. Executor
Carries out the finalized execution.

Responsibilities:
- Execute trades or transfers
- Report execution results
- Settle outcomes

---

Only validated intents may progress through all roles.
