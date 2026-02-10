# Day 15 – External Rule Configuration

## What changed
- Moved QA rules into an external JSON-style config
- Updated the engine to consume rules as data

## Why this matters
- Standards can change without code changes
- Rules can be shared across projects or teams

## Connection to ACC / APS
- Rules can come from APIs or project settings
- Engine logic maps cleanly to backend services

## What feels solid now
- Treating rules as data and keeping the engine generic.

## What I want to explore next
- Loading rules dynamically instead of simulating them in code.
