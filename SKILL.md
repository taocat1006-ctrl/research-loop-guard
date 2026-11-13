
---
name: research-loop-guard
description: >-
  Keep research iterations bounded and tied to decisions. Use when planning the next
  experiment, deciding whether to continue or stop, reviewing a stalled project, or
  diagnosing repeated evidence gathering and restarts. Connect questions, evidence,
  and cumulative effort to an explicit decision. Ordinary paper summaries and
  isolated code fixes do not need the full workflow.
---

# Research Loop Guard

Make exploration produce knowledge that can inform a decision. Having more work available is not, by itself, a reason to continue. Support promising ideas without dismissing an entire direction because of related work, one failed version, or results that are not yet publishable.

This skill governs research decisions. It does not authorize model calls, external communication, unattended continuation, or delegation. Follow the user's current instructions and complete already authorized work within its budget without asking for confirmation at every step. Previously stopped branches require the treatment below.

## Recover the decision before running another experiment

Find the current question, recent results, and latest stop decision. Reuse existing protocols, analyses, and raw outputs. Distinguish historical suggestions from current decisions: a next step in an old report is not automatically authorized.

Check the project's latest effective decision and whether the user has explicitly changed it. Do not turn one version's failure into a verdict on the entire research direction. Consult the [behavior examples](references/behavior-examples.md) when a typical situation needs clarification; these examples do not establish the current project's status.

Classify the current work. If the state is unclear, inspect only the records needed to resolve it.

| State | Action |
|---|---|
| Exploring; no specific question yet | Look for concrete differences, combinations, and counterexamples within a bounded set of materials. Descriptive observations are valid; do not build a complete framework first. |
| A testable question exists, but no result distinguishes the main explanations | Choose one bounded experiment most likely to change the decision to continue. |
| Existing results are sufficient for the current decision | Explain the results and decide. Do not add checks merely for reassurance. |
| A technical failure prevented a valid test | Separate the failure from the scientific question and use the agreed repair budget. |
| A budget or stopping condition has been reached | Close the branch. Do not automatically turn each error into another research task. |

## Write one short decision card

Reuse the project's records. If none exist, use the [decision card template](references/decision-card.md). Do not create a separate management system for this skill. A normal iteration needs roughly half a page to one page covering:

1. **Parent question and current question.** Which single uncertainty does this iteration address, and why does it determine progress on the parent question?
2. **What the result changes.** State the action for supporting, opposing, and inconclusive results. If every outcome leads to more experiments, the iteration lacks a decision purpose.
3. **Fit between evidence and claim.** What level of question can the materials, controls, and evaluation answer? How would a successful output differ from plausible alternative explanations?
4. **Minimum execution and total budget.** Specify materials, primary observations, call/sample/time limits, and permitted technical repairs. Carry forward cumulative effort on the parent question; renaming the task or changing folders does not reset it.
5. **Completion and stopping conditions.** State when the evidence is sufficient, when to stop, and when uncertainty is the only justified conclusion. Base thresholds on the task; do not invent a zero-error standard during execution.

Exploration does not require knowing the pattern in advance or completing a statistical test design first. It does require a bounded observation scope and a concrete deliverable: for example, source-supported recurring combinations and counterexamples, followed by a decision on whether to formulate a hypothesis. Open exploration does not waive the budget.

If no budget is specified, state a conservative limit proportionate to the task, make assumptions explicit, and proceed within existing authorization. For a stopped branch, first provide a concrete restart rationale; do not resume experiments under a self-assigned default budget.

If historical expenditure cannot be recovered reliably, record it as unknown, retain any known lower bound, and cap the remaining effort from now on. Do not launch a historical investigation just to fill in the budget field.

## Prefer work that can change the parent decision

Before acting, answer in one sentence: **How would different outcomes of this step change our research judgment?**

- More citations, fields, examples, audit files, or cleaner figures do not automatically add knowledge. Necessary engineering is legitimate; label it as engineering and define its delivery boundary.
- A component experiment must identify which obstacle to the parent question its result can rule out. A better component score does not establish the overall claim or justify a top-tier submission.
- Start with existing methods, prompts, and materials. A custom method needs a specific unmet need and a clear contribution. Do not describe a custom adaptation as an exact reproduction.
- When related work exists, compare the closest work's actual mechanisms, inputs, objectives, and limitations. Develop substantive differences where they exist; otherwise explain the overlap and possible adjustments. Verify specific points instead of searching indefinitely for proof that nobody has ever tried the idea.
- Among candidate next steps, choose the one with the greatest current decision value. Other ideas may remain as brief backlog notes; do not execute them automatically or build a chain of derivative studies.

## Prevent the target from moving during execution

Preserve original inputs, outputs, rules, and versions. Explain how each change affects the question being tested.

- A technical rerun repairs the original comparison only when the task, model, budget, and evaluation remain the same. Keep failures and do not select only successful responses. Unless otherwise agreed, allow one bounded repair batch supported by a specific diagnosis, then close the iteration.
- Changes to prompts, models, granularity, corpora, labels, evaluation rules, or output limits may be valid development, but create new development conditions. Charge them to the parent budget. Do not overwrite the original results or present them as the original frozen evaluation.
- After inspecting answers, failure cases, or human corrections, label subsequent results on the same materials as development or retrospective results. Do not call them independent validation. Keep human-supplied corrections separate from automated output.
- Check only unresolved issues that could change the conclusion. Once the main conclusion and necessary validation are established, deliver. Do not create an audit of the audit in pursuit of perfect evidence.
- If an iteration adds detail without advancing the parent question, state that the decision has not changed. Do not automatically replace the next step with an even smaller component question.

## Separate four kinds of conclusions

| Conclusion | Justified statement | Next action |
|---|---|---|
| Supported within the current scope | Specify the objects, conditions, actual gain, and remaining alternative explanations. | Follow the planned continuation decision or deliver. Do not promise publication acceptance. |
| A valid test did not meet the threshold | This version did not meet the requirement on this task. | Stop or redirect as planned. Do not automatically add rescue experiments. |
| Insufficient or mixed evidence | State what remains indistinguishable; do not treat uncertainty as either an effect or no effect. | Add work only if the original budget permits it and it can resolve the key ambiguity; otherwise close with uncertainty. |
| No valid test was completed because of technical failure | Describe the fault, coverage, and missing data. This does not refute the scientific claim. | Attempt bounded repair; if recovery fails, close the iteration. |

Descriptive findings can be valid intermediate results. Every observation need not satisfy the proof standard of a complete paper. Conversely, examples, candidates, and human curation cannot be promoted into general laws.

## Make stopping effective

Stop automatic expansion of the branch and deliver the existing conclusion when any of the following holds:

- A predefined failure threshold, time/call/sample budget, or explicit user stop instruction has been reached.
- The proposed next step still cannot distinguish the main explanations, or the evaluation target does not match the claim.
- Two consecutive iterations add representations, materials, checks, or components without changing the research decision on the same parent question. This is the skill's default stopping rule; the user may adjust it in advance. A new chat, name, or directory still belongs to the same research chain.

After stopping, do not turn every discovered error into an executable task. Near-success, remaining model errors, a desire for one more check, or available money and compute are not sufficient reasons to continue.

A restart proposal must specify the new information or grounded intervention, why it could resolve the previous key uncertainty, the smallest experiment that distinguishes the explanations, which prior failures remain relevant, and the maximum new investment. Fixing extraction, adding fields, or changing models may be an intervention, but naming a change is not a rationale: connect it to the failure mechanism and parent question. A restart must be open to rejection; renaming the question must not bypass a stop decision.

For a branch explicitly stopped by the user or under an agreed project decision, present that concrete proposal and wait for an explicit restart instruction. Cite this requirement and the original stop basis to explain why execution cannot simply resume. Do not extend this requirement to ordinary authorized iterations. Organizing results, explaining, writing, and maintaining this skill do not restart experiments.

If the current user has already explicitly requested a restart and specified the action, that instruction is authorization. Record the new scope, rationale, and bounded budget, then execute without asking again. A feasibility question or general expression of concern is not a restart instruction.

## Respect evidence boundaries and deliver

Preserve distinctions relevant to the current question; do not generate extra experiments just to complete a checklist.

- A citation match is not semantic support. Similar operations do not establish that entire methods are structurally equivalent or interchangeable.
- Identify the provenance of human curation, model outputs, and external annotations. Independent experts are not universally required, but self-review is not independent evidence.
- Reproducing a known case is not discovering a new analogy. If the source states the connection or model memory remains a plausible explanation, do not claim that knowledge leakage has been ruled out.
- Samples from the same source, variants, and exhaustive table entries are not independent papers. Do not directly compare success rates when systems have different coverage.
- No observed gain does not prove ineffectiveness. One failed version does not establish impossibility. A local result is not a universal law.

End each iteration with **result, scope of support, decision, and cumulative expenditure**, linked to the key raw evidence. Answer the research question before recounting execution details. Multiple report formats are not required for every iteration. A small reliable finding, a valid counterexample, a clear statement of uncertainty, or a stop decision can each be a useful deliverable.

When asked whether a direction is worth pursuing or has become a loop, give an objective assessment and explanation first. Do not substitute reassurance for judgment or start experiments in response to anxiety. This skill reduces uncontrolled iteration; it cannot guarantee research success or acceptance at a top-tier venue.
