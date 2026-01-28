# Day 3 – Data Structures (AEC Context)

## Key idea
Programs mostly move data around.
The way data is organized determines what is easy or hard to do.

---

## Core data structures (conceptual)

### 1. List (Collection / Array)
What it is:
- An ordered collection of items

AEC example:
- A list of all walls in a model
- A list of all issues in an ACC project

What it’s good at:
- Looping through items
- Counting
- Simple checks

What it’s bad at:
- Finding one specific item quickly

---

### 2. Dictionary (Key–Value pairs)
What it is:
- A lookup table where each key maps to a value

AEC example:
- ElementId → Element
- Parameter name → Parameter value
- User email → Role

What it’s good at:
- Fast lookups
- Mapping relationships

What it’s bad at:
- Ordering
- Duplicates (keys must be unique)

---

### 3. Nested data
What it is:
- Data structures inside other data structures

AEC example:
- Project
  - Models
    - Elements
      - Parameters

Why this matters:
- BIM data is always nested
- APIs expose nested data constantly

---

## Exercise: Model Health Data Design (No code)

If I were storing model health results, I might use:

- A list of elements
- Each element has:
  - Element ID
  - Category
  - A dictionary of parameter checks
  - A list of failed rules

Reason:
- I need summaries AND detailed drill-down

---

## Dynamo connection
In Dynamo:
- Lists = obvious
- Dictionaries = less obvious but powerful
- Nested lists = common source of confusion

---

## Reflection
What clicked today:
- List vs Dict pros and cons

What still feels fuzzy:
- It still feels pretty simple and easy to understand
