# Behavioral Eval Runs

Recorded model-behavior evaluations live here, separate from Ralph iteration logs and code-generation traces.

Each dated run folder contains the exact prompts, full model outputs, run metadata, and a rubric-based scorecard. These are evidence snapshots, not a promise that every model/version will behave identically.

- `2026-11-25-gpt-6-luna-full-suite/` — all 11 Socratic Teacher scenarios, with extensions and auto skill discovery disabled, the skill explicitly loaded, and write tools enabled. Result: 11/11 passed. See the scorecard for the case 8 plan-context setup and residual risk around post-approval file writes.
