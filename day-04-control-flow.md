# Day 4 – Control Flow (AEC Context)

## Key idea
Programs don’t think.
They follow instructions in order, one step at a time.

Control flow decides:
- What runs
- When it runs
- How often it runs

---

## 1. Loops (Repeat work)

What it is:
- A way to repeat the same action for many items

AEC example:
- For each wall in the model:
  - Check parameters
  - Validate naming
  - Record issues

Why loops matter:
- Models have thousands of elements
- You never check things one-by-one manually

Common mistake:
- Forgetting what happens when the list is empty
- Forgetting what happens when there are 100,000 items

---

## 2. Conditions (If / Else logic)

What it is:
- A decision point

AEC example:
- If a required parameter is missing:
  - Flag an issue
- Else:
  - Continue

Why this matters:
- Most automation is just rules
- Rules are conditions

---

## 3. Loop + condition together (real power)

AEC example:
- For each element:
  - If category is Wall:
    - Check fire rating
  - If category is Door:
    - Check width
  - Else:
    - Skip

This is how one tool handles many cases.

---

## Dynamo connection

In Dynamo:
- Loops are hidden inside nodes
- Conditions are often Boolean nodes
- Complex graphs = hidden control flow

Why code feels “simpler” later:
- Control flow becomes explicit

---

## Reflection

What felt obvious:
- Most dynamo scripts I have authored in the past have been loop + condition

What felt unintuitive:
- Nothing yet
