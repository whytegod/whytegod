# Intent Validation Rules

All execution intents MUST satisfy the following rules:

## Required Fields
- intent_id
- requester
- asset
- amount
- constraints
- destination
- expiry

## Constraints
- amount MUST be greater than zero
- expiry MUST be a future timestamp
- asset MUST be supported by the execution layer
- constraints MUST be explicit

## Rejection Conditions
- Expired intent
- Invalid schema
- Unsupported asset
- Constraint violation

## Acceptance
Only validated intents are admitted into the execution flow.
