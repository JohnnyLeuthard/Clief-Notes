# Vault Naming Standards

[PLACEHOLDER — Add your organization's CyberArk naming conventions here]

## What to Include

- Safe naming patterns (prefix, delimiter, suffix rules)
- Platform naming conventions
- Account naming rules per platform type
- Any exceptions or legacy patterns to account for

## Why This File Matters

This is Layer 3 shared reference material. Multiple stages across both EVD and psPAS pipelines load this file:
- EVD/01_sql_gen uses it to interpret data values when writing SQL
- EVD/03_parsing uses it to check accounts for compliance
- psPAS/01_planning uses it to determine the correct target values when remediating

It is configured once during workspace setup and stays the same across every run.
