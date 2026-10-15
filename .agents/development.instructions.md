---
name: Development Rule
description: Keep development changes focused and verify them with the narrowest relevant check.
applyTo: "**"
---

# Development Rule

## Scope

This rule is always active for every file in the repository through the `**` file pattern. It does not require the agent to be explicitly invoked.

## Rule

Before changing code or configuration, inspect the nearest relevant implementation and its local conventions. State a concrete expectation for the change and identify a focused check that could disprove it. Make the smallest change that addresses the task, preserve unrelated user changes, and run that focused check immediately after editing. Do not broaden the change or validation scope unless the check reveals a specific need.
