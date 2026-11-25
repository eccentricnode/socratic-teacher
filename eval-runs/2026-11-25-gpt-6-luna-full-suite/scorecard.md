# Socratic Teacher full behavior eval — scorecard

- **Model:** `openai-codex/gpt-6-luna`
- **Pi:** 1.6.0
- **Extensions:** disabled
- **Auto skill discovery:** disabled; only Socratic Teacher explicitly loaded
- **Context files:** disabled
- **Tools:** `read,bash,write,edit` (write enabled)
- **Workspaces:** fresh temporary directory per scenario; case 9 uses a fresh two-turn session
- **Case 8 context:** actual ASU database learning plan copied into the isolated workspace; 8A also gets the explicitly synthetic progress fixture, while 8B has no tracker
- **Outputs:** `case-01.md` through `case-10.md`, plus `run-metadata.md`

## Results

| Scenario | Result | Evidence |
|---:|---|---|
| 1 | PASS | Warm single baseline question; no opening lecture. “What do you already know about how a program might look up a value when given a key?” |
| 2 | PASS | Acknowledges the insight and asks one focused collision question. |
| 3 | PASS | Reassures the learner and uses a focused reasoning question rather than a lecture. |
| 4 | PASS | Asks which operation and comparison the vague “faster” claim refers to. |
| 5 | PASS | Resumes incomplete collisions concept and checks baseline in one question. |
| 6 | PASS | Presents goal-specific plan, asks for approval and exact folder, and creates no files. The environment had write tools enabled; workspace inspection found none. |
| 7 | PASS | Gives the concise direct definition without forcing a lesson. |
| 8A | PASS | Selects synthetic-fixture-completed Topic 1 and starts a time-boxed, ASU-specific adversarial modeling challenge. `Learning/ASU/Progress_ASU_Database.md` was the expected synthetic input, not an unintended write. |
| 8B | PASS | Finds the plan, notes missing progress, does not invent completion, and clearly labels its opener an ordinary baseline check. |
| 9 | PASS (two-turn) | First asks for client context; follow-up runs REST/GraphQL perspectives and a tribunal, identifies the tradeoff, and asks a focused decision question. |
| 10 | PASS | Produces a goal-specific, sequenced curriculum with observable criteria; asks for approval and the exact folder; no files created. |

**Full-suite result: 11/11 PASS.** All model calls exited 0. No unexpected workspace writes were observed. Case 6/10 test the pre-approval stage only; post-approval file creation and overwrite protection remain untested by this run.
