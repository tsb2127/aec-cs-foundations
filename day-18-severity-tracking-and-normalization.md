# Day 18 – Severity Tracking + Safer Normalization

## What changed today

- Added severity counting (warning vs error)
- Normalized Dynamo / .NET collections safely before counting
- Cleaned rule evaluation to return both issues and severity stats
- Reduced silent failures from DesignScript list types

## What clicked

Dynamo inputs are not normal Python objects.

Some are:
- DesignScript collections
- .NET collections
- Single objects
- Null

The script must normalize everything before applying logic.

This is the difference between writing code
and writing defensive production code.

## What feels stronger now

The engine now:
- Counts elements safely
- Evaluates rules cleanly
- Tracks severity levels
- Produces structured output

It feels more like a real QA engine now.

## What I want to refine next

- Add configurable fail logic (fail only on "error")
- Add rule types beyond min_count
- Support thresholds (e.g. max_count)
- Export report to JSON file
