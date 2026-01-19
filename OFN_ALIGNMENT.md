# WHYTGOD × Open Financial Network (OFN)

## Relationship Overview

WHYTgod is an AI-first, peer-to-peer financial execution layer designed to operate
on top of the Open Financial Network (OFN).

OFN provides the foundational financial primitives, settlement rails, and trust
assumptions. WHYTGOD does not replace OFN — it coordinates, routes, and executes
intents within the OFN environment.

## Nature of Alignment

- OFN is the base financial network
- WHYTGOD is an execution and intelligence layer

WHYTgod consumes OFN-compatible intents, assets, and routing rules while remaining
protocol-agnostic at the interface level.

## Design Dependency

WHYTgod assumes:
- OFN-compliant asset definitions
- OFN settlement finality
- OFN security guarantees

If OFN evolves, WHYTGOD adapts without breaking compatibility.

## Non-Claims

WHYTgod does not:
- Claim ownership of OFN
- Represent OFN governance
- Modify OFN consensus or settlement logic

WHYTgod is an execution consumer, not a base-layer authority.

## Rationale

This separation preserves institutional trust, regulatory clarity,
and long-term protocol safety.
