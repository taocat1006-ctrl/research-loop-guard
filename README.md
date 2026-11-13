# Research Loop Guard

A Codex skill for deciding when to continue, redirect, or stop a research iteration.

Research can stall even while every individual task looks productive: another extraction fix, another evaluation field, another round of evidence. Research Loop Guard ties each iteration to a question, a decision, and a cumulative budget so that activity does not substitute for progress.

## What it does

- Recovers the current question, existing evidence, and latest effective decision before starting another experiment.
- Uses a short decision card to define the question, evidence, outcome-dependent actions, budget, and stopping conditions.
- Tracks effort against the parent research question across iterations, chats, and renamed experiments.
- Separates technical failure, development results, independent validation, and scientific evidence.
- Stops automatic expansion after two consecutive iterations that add components or materials without changing the parent decision; users can adjust this default in advance.
- Requires a concrete rationale to restart a stopped branch, while honoring an explicit restart instruction without asking again.

## When to use it

Use it to plan the next experiment, assess a stalled project, decide whether another check is worth doing, or review a proposed restart. Ordinary paper summaries and isolated code fixes do not need the full workflow.

The aim is useful knowledge and a justified decision. A descriptive finding, a counterexample, or a clear account of uncertainty can all be valid outcomes.

## Installation

Clone the repository into your Codex skills directory:

```bash
git clone https://github.com/taocat1006-ctrl/research-loop-guard.git ~/.codex/skills/research-loop-guard
```

If you use a custom `CODEX_HOME`, use its `skills` directory instead. If the destination already exists, preserve or back up your existing version before deciding how to merge it. Start a new Codex session to load the skill.

## Usage

```text
Use $research-loop-guard to review our existing records and decide whether
another research iteration is worthwhile. Define the question, budget,
and stopping conditions for any justified next step.
```

Other useful requests:

- "Are we learning something new, or just patching the same failed approach?"
- "Do the current results already support a decision?"
- "Is there enough new evidence to justify restarting this branch?"

## Repository contents

| File | Purpose |
|---|---|
| [SKILL.md](SKILL.md) | Core research decision rules. |
| [references/decision-card.md](references/decision-card.md) | A reusable decision card for one iteration. |
| [references/behavior-examples.md](references/behavior-examples.md) | Hypothetical scenarios and expected behavior. |
| [agents/openai.yaml](agents/openai.yaml) | Codex display metadata and default prompt. |

## Scope

This is a general-purpose release without private project records or local evidence paths. Examples are illustrative, not independent evaluation results. The skill governs research decisions; it grants no additional execution permissions and does not guarantee research success or publication acceptance.
