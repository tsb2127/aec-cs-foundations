# Day 5 – Errors, Failure, and Edge Cases

## Key idea
Automation does not fail randomly.
It fails at boundaries, assumptions, and missing cases.

Professionals expect failure and design for it.

---

## Types of failure (conceptual)

### 1. Missing data
What it is:
- Something you assumed exists… doesn’t

AEC examples:
- A required parameter is not bound
- A model has zero elements of a category
- An ACC project has no issues yet

Why this breaks automation:
- Code tries to read something that isn’t there

---

### 2. Unexpected data shape
What it is:
- Data exists, but not in the form you expected

AEC examples:
- Parameter value is text instead of number
- Units are inconsistent
- Nested data is deeper than expected

Why this breaks automation:
- Logic assumes a specific structure

---

### 3. Scale problems
What it is:
- Logic works on small models, fails on large ones

AEC examples:
- 50 elements vs 50,000 elements
- Single model vs multiple linked models

Why this breaks automation:
- Performance assumptions were wrong

---

### 4. Ambiguous rules
What it is:
- The rule sounds clear to humans, not to computers

AEC examples:
- “Check naming consistency”
- “Ensure model quality”
- “Validate standards”

Why this breaks automation:
- Rules were never made explicit

---

## Edge cases (where professionals think)

Examples:
- Empty model
- Partially complete model
- Model mid-design vs issued-for-construction
- ACC project with restricted permissions

Edge cases are not rare.
They are normal.

---

## CS50 Lecture 0 – Connection

Key takeaway:
- Scratch is kinda like Dynamo with some more features like sound and movement along (xy plane)

Connection to BIM:
- Better to modularize code as much as possible
- Assumptions must be surfaced

---

## How this changes how I think

Before:
- Learning landuages/syntax felt like too much unnecessary work

Now:
- What's more important - logic, efficiency, edge cases, failures & assumptions
- Launguage / Syntax can just be copy pasted

---

## Reflection

One failure I’ve seen in real AEC workflows:
- Most Dynamo scripts seem to be inefficient

One assumption I often make that could break automation:
- It working for one example is easy. Making it scalable introduces edge cases and breaks automation
