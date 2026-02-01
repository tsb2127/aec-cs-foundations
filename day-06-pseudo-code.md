# Day 6 – Pseudo-Code (AEC Automation)

## Key idea
Pseudo-code is how you design logic before choosing a language.
Good pseudo-code makes coding boring.

---

## Example 1: Model Health Checker (Read-only)

GOAL:
Check a model for missing parameters and naming issues.

PSEUDO-CODE:

START
  Open model

  Get list of all elements

  IF element list is empty
    Report "No elements found"
    STOP

  FOR each element in element list
    IF element category is not relevant
      CONTINUE

    FOR each required parameter
      IF parameter does not exist
        Record issue (missing parameter)
      ELSE IF parameter value is empty
        Record issue (empty value)

    IF element name does not match naming rules
      Record issue (naming violation)

  END FOR

  Summarize issues
  Output results
END

## Example 2: ACC Project Data Check

GOAL:
Extract basic health info from an ACC project.

PSEUDO-CODE:

START
  Connect to ACC project

  Get project metadata
  Get list of models
  Get list of issues

  IF no models exist
    Record warning

  IF no issues exist
    Record informational message

  FOR each model
    Record model name
    Record last updated date

  Output summary report
END
