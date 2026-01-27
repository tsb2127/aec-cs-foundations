# Day 2 – Thinking Like a Programmer

## Key idea
Code is not magic.
It is written instructions that remove ambiguity.

Before writing code, you must make decisions explicit.

---

## Exercise 1: Model Health Check (Conceptual)

### Goal
Check a BIM model for issues before publishing.

### Inputs
- A BIM model
- A list of required parameters
- A naming standard

### Outputs
- A list of issues
- A summary count of problems

### Step-by-step logic (no code)
1. Open the model
2. Find all relevant elements
3. For each element:
   - Check if required parameters exist
   - Check if parameter values are filled
   - Check naming rules
4. If a rule fails, record an issue
5. At the end, summarize results

---

## Exercise 2: Why ambiguity is dangerous

Example:
"Check all walls"

Questions a computer would ask:
- What counts as a wall?
- What model?
- What does "check" mean?
- What is a failure?

### Lesson
Computers fail where humans assume context.

---

## Reflection
What surprised me:
- Nothing really. The logic matches how I already think when building a dynamo script for example.

What felt unclear:
- Nothing yet.
