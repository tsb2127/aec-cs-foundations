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

## CS50 Lecture 3 – Algorithms (Notes)
Finished CS50 Lecture 3. A few things stood out:

- Linear vs binary search made it clear how much data structure choices matter.
  Once data is structured, logic becomes simpler and more efficient.

- Selection, bubble, and merge sort showed the tradeoff between simplicity and performance.
  This feels similar to separating rules from the engine before worrying about optimization.

- Big-O and Ω notation reframed performance as a design decision.
  The rule engine here is simple by design, but structured so it can scale without a rewrite.

- The recursion example (and the recursive Google search joke)

Overall, this reinforced that good automation design starts with structure, not clever code.
