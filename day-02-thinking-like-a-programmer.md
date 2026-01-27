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

## Exercise 3: Making rules explicit

Original rule:
"Check if the model is ready for publishing."

Rewrite as explicit checks:
- The model contains no warning-level errors
- All required parameters exist on required categories
- All sheets have approved status
- No elements exist on forbidden worksets

### Lesson
Vague goals must become testable rules.

---

## Exercise 4: Thinking in failure cases

If this automation fails, possible reasons:
- The model is workshared and not editable
- Parameters exist but are not instance-based
- Elements are in linked models
- User permissions block access

### Lesson
Most automation bugs come from assumptions, not syntax.

---

## CS50 – Lecture 0 takeaway
- Reinforced that computers only do exactly what they’re told
- Matches why ambiguity breaks automation
- Confirms why logic-first thinking matters before APIs


## Questions I expect code to answer later
- How do I reliably get all elements of a category?
- How do I detect missing vs empty parameters?
- How do I report issues without modifying the model?
- How do I make this fast on large models?


## Reflection
What surprised me:
- Nothing really. The logic matches how I already think when building a dynamo script for example.

What felt unclear:
- Nothing yet.
