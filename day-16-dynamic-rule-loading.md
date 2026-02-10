# Day 16 – JSON-Driven Model Health Engine (Dynamo + Python)

## What I built
A small but real **model health engine** in Dynamo using Python, where:

- Revit elements (Walls, Doors) come in from Dynamo
- QA rules are defined externally in a JSON file
- The Python script evaluates counts against those rules
- The output is a structured report (counts + issues)

This is the first time the graph felt like an *engine*, not a script.

---

## Core idea
**Separate logic from configuration.**

- Dynamo = data acquisition
- Python = evaluation engine
- JSON = rules + thresholds

Changing QA logic now means editing JSON, not touching code.

---

## Inputs
- `IN[0]`: Walls (list from *All Elements of Category*)
- `IN[1]`: Doors (list from *All Elements of Category*)
- `IN[2]`: Parsed JSON rules (via `Data.ParseJSON`)

---

## What clicked today
- Dynamo data types are *not* normal Python types  
- You must normalize inputs before doing real logic
- Defensive coding is not optional at API boundaries
- JSON-driven rules feel very similar to real QA / linting systems

This finally explains why earlier scripts kept breaking in confusing ways.

---

## What was hard
- Errors caused by Dynamo’s internal object types
- `len()` failing even when things “looked like lists”
- Debugging required inspecting **types**, not values

This was frustrating, but also very clarifying.

---

## Why this matters
This same pattern is used in:
- QA engines
- Linting tools
- CI validation
- ACC / APS automation pipelines

This doesn’t feel like “Dynamo stuff” anymore — it feels like software.

---

## What I want to expand next
- Add element-level checks (parameters, nulls, naming)
- Split warnings vs errors more intentionally
- Eventually port this logic to a non-Dynamo environment

---

## Files added today
- `model-health-engine.dyn`


