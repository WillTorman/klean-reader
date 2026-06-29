# ADR 0001: Use TypeScript

- Date: 2026-06-28
- Status: Proposed

## Context

The repository will host multiple clients (web now, mobile later). Shared logic is expected.

## Decision

Use TypeScript for app and shared code.

## Consequences

### Positive

- Stronger contracts across apps
- Safer refactors
- Better editor tooling

### Negative

- Slightly more setup and type maintenance

## Follow-Up

- Define baseline tsconfig standards
- Decide strictness level for initial phase
