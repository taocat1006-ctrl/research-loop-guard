# Behavior Examples

These hypothetical scenarios illustrate the skill's research decisions. They are not records from a particular project, evaluation results, or evidence that the current project has stopped.

| Scenario | Expected behavior |
|---|---|
| A prototype missed a preregistered threshold. "Could changing the granularity make it work?" | Discuss feasibility and connect the intervention to the failure mechanism. If the branch has stopped, propose a bounded restart and wait for an explicit restart instruction. |
| "Restart explicitly: change the granularity for one more iteration, without expanding the sample." | Treat the instruction as authorization. Record the conditions, rationale, and budget; preserve prior failures; execute only this iteration. |
| An API timed out. "Does this mean the direction is invalid?" | Separate technical failure from scientific failure. Use the agreed repair budget; do not infer that the scientific claim has been refuted. |
| "Checking ten more papers would be safer." | Identify a specific unresolved issue that could change the decision. If none exists, deliver the current conclusion. |
| Experiments have stopped, but the user requests a report on existing results. | Complete the writing within existing evidence. Reporting is not a restart and does not authorize new experiments. |
| Closely related work exists. | Compare mechanisms, inputs, objectives, and limitations. Develop substantive differences; acknowledge overlap honestly. |
| The goal is to explore recurring combinations, without yet claiming that a model beats a baseline. | Bound the observation scope, preserve source evidence and counterexamples, and allow a descriptive finding to close the iteration. |
| Two iterations only identified more fields to add; a renamed experiment is proposed. | Accumulate effort under the same parent question and apply the default stopping rule. Renaming does not reset the budget. |
| Conditions have different successful-response coverage, but someone wants to compare success rates directly. | Explain missingness and coverage differences. Inconsistent denominators do not establish a comparable effect. |
| A prompt is revised after reviewing failures and improves on the same materials. | Label the result as development or retrospective evidence. Preserve the original results; do not call this independent validation. |

## Transferable lessons

- Bounded component experiments do not ensure a bounded parent investigation. Track cumulative effort across the research chain.
- A component improvement does not automatically support the overall claim. State how different outcomes would change the parent decision before execution.
- A locatable citation does not necessarily support the claim. Human corrections must not be counted as automated successes.
- Failure can identify one version's limits without invalidating the entire direction. Preserving a direction does not justify manufacturing success.
