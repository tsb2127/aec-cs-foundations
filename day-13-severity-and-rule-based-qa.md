# Day 13 – Severity Levels & Rule-Based QA

## What changed
- Introduced severity levels (info, warning, error)
- Replaced generic warnings with structured issues

## Why this matters
- Makes reports actionable instead of descriptive
- Enables filtering, alerting, and automation

## Connection to ACC / APS
- QA systems rely on severity-based issues
- This structure maps cleanly to issue APIs

## What feels solid now
- Designing outputs that can be filtered and acted on by downstream systems.

## What I want to refine next
- Aligning these rules with how ACC / APS issue workflows are modeled.

## Additional progress (extended session)

Spent extra time solidifying ACC / APS fundamentals, including:
- APS 2-legged OAuth flow working end-to-end
- ACC app authorization correctly configured
- Hub → Project resolution clarified and repeatable
- ACC Docs topology understood (Projects API vs Data API)
- Folder traversal via IDs (not paths)
- Postman post-response scripting to manage environment state
- Also continued CS50 Lecture 2 (arrays), reinforcing list-based thinking used throughout this work.
