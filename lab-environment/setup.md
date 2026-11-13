# Lab Setup Plan

## Initial approach

Start with a small local application that simulates an AI assistant and a few deliberately insecure design choices. The lab must use synthetic data and simulated tools only.

## Proposed components

- Local Python application
- Mock assistant logic (initially deterministic; no external model/API required)
- Synthetic system instructions and documents
- Simulated tools with harmless local-only effects
- Test runner that records input, output, and tool-call decisions
- Sanitized evidence directory

## Why begin without a live model?

A deterministic mock makes expected behaviour and test outcomes easier to reproduce. Once the testing harness works, a model-backed mode can be added with explicit configuration and cost/safety controls. Do not send sensitive data to external model providers.

## Environment requirements

- Windows, macOS, or Linux
- Python 3.11 or later
- Git
- A code editor

## Planned setup sequence

1. Verify Python and Git installations.
2. Create and activate a virtual environment.
3. Add the local lab application and test harness.
4. Run baseline tests.
5. Add one vulnerability scenario at a time.
6. Capture sanitized logs and document results.

No tests have been run yet. This file describes the planned environment, not a completed deployment.
