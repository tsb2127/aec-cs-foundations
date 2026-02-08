# Day 14 – Config-Driven QA & Correct Severity

## What changed
- Refactored QA checks into a config-driven rule structure
- Separated rule definitions from the execution engine
- Corrected severity semantics to reflect domain context

## Why this matters
- Rules can evolve without changing core logic
- Severity reflects impact, not just missing data
- Output structure is stable and API-ready

## Connection to ACC / APS
- Rules map to org or project standards
- Engine maps to backend validation services
- Report structure aligns with JSON-based APIs

## What feels solid now
- Designing config-driven rules and applying them through a generic engine.

## What I want to explore next
- Defining checks that genuinely deserve error-level severity.
