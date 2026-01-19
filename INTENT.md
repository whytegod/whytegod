# WHYTGOD Execution Intent

## Intent Definition
An Intent is a signed instruction describing
what outcome the user wants — not how to execute it.

## Core Fields
- intent_id
- requester
- asset
- amount
- constraints
- risk_profile
- destination
- expiry

## Properties
- Stateless
- Non-custodial
- Deterministic
- Verifiable

## Execution Rule
WHYTgod interprets intent.
OFN executes settlement.
No party mutates intent.

## Example (Abstract)
User wants to move value
→ defines intent
→ WHYTGOD routes
→ OFN settles
