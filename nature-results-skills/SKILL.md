---
name: nature-results-skills
description: Rewrite, polish, and audit biomedical or life-science manuscript Results subsections in a Nature/Science style. Use when Codex is asked to improve Results text from figures, figure legends, panels, tables, or user-provided experimental summaries; enforce premise-findings-conclusion structure, problem-driven logic, precise figure anchoring, controlled interpretation, rigorous controls/statistics, and iterative self-review until the Results claim matches the data.
---

# Nature Results Skills

## Core Workflow

Use this skill to turn a data-described Results section into a question-driven, figure-guided, reviewer-resistant Results narrative.

Follow this sequence:

1. Identify the scientific question, the main claim, the figure panels, and the evidence type.
2. Rewrite the Results using the three-part unit: Premise, Findings, Conclusion.
3. Reorder the narrative from data-driven chronology to problem-driven logic.
4. Audit the rewrite with the Results review rubric.
5. Revise again if any audit gate fails.
6. Return the final Results text plus concise notes on major changes and residual limitations.

For detailed audit criteria, read `references/review-rubric.md`.

## Input Handling

When the user provides figure images, inspect the visual evidence before rewriting. Extract only what the figure supports: panel labels, comparison groups, direction of effect, statistical labels, controls, and obvious inconsistencies.

When the user provides both text and figures, check whether the text overstates or misreads the figures. Prefer the figure evidence over unsupported wording.

When evidence is incomplete, write conservatively and mark missing items, such as absent `n`, missing statistical test, unclear control, unclear sample type, or missing panel legend.

## Rewriting Rules

Structure each subsection or major result as:

- Premise: one sentence explaining why the experiment or analysis was done.
- Findings: objective, figure-anchored description of what was observed.
- Conclusion: one restrained sentence explaining what the result means for the story.

Use problem-driven order when possible:

1. Phenomenon: establish the observation.
2. Association: identify candidate factors or programs linked to the observation.
3. Necessity: show loss-of-function, inhibition, depletion, knockout, knockdown, or rescue evidence.
4. Sufficiency: show gain-of-function, overexpression, activation, reconstitution, or transfer evidence.
5. Mechanism: explain molecular, cellular, physical, or computational mechanism.

Do not force this full chain if the data do not contain it. Instead, expose the missing causal step as a limitation or future validation need.

## Figure Guidance

Make the prose a guide to the figure, not a repetition of every value.

- Anchor key findings to exact panels, such as `Fig. 1, B and C`, `Extended Data Fig. 2a`, or `Table S1`.
- Report exact numbers only when they are central, surprising, needed for scale, or not visually obvious.
- Avoid listing long gene/protein/metabolite sets in the main text; move them to tables or supplementary references when possible.
- Keep main-figure claims central. Assign routine validation, method checks, and technical controls to supplementary figures unless they support the core claim.

## Language Rules

Use restrained, precise language.

- Use past tense for the authors' experiments and findings: `We found that...`, `Treatment reduced...`.
- Use present tense for figure presentation and established facts: `Figure 2 shows...`, `EGFR is a receptor tyrosine kinase`.
- Avoid subjective adjectives such as `astonishingly`, `spectacular`, `strikingly`, or `dramatically` unless the user explicitly requests a more rhetorical style.
- Replace causal language with associative language unless causality is directly tested.
- Keep clinical or translational claims out of Results unless supported by clinical data.

Useful verbs by evidence strength:

- Association only: `was associated with`, `was enriched in`, `was linked to`, `nominated`, `prioritized`.
- Perturbation evidence: `reduced`, `increased`, `impaired`, `restored`, `rescued`.
- Causal evidence with necessity and sufficiency: `was required for`, `was sufficient to`, `mediated`.

## Rigor Requirements

Actively mention rigor when it strengthens the result:

- Negative controls: vehicle, mock, scramble, isotype, untreated, wild-type, empty vector.
- Positive controls: known inducer, inhibitor, marker, benchmark, or validated reference.
- Statistics: biological replicates, statistical test, confidence intervals, effect direction, multiple-testing correction for high-throughput data.
- Boundaries: weaker effects in a model, non-significant panels, assay limitations, cohort size, in vitro-only evidence, or lack of causal validation.

Do not invent controls, statistics, sample sizes, or panel contents. If absent, flag them as missing.

## Audit-And-Revise Loop

After the first rewrite, review it against these gates:

1. Visual-only gate: Would the figure panels independently support the narrative?
2. Logic-chain gate: Does the text distinguish phenomenon, association, necessity, sufficiency, and mechanism?
3. Rigor gate: Are controls, statistics, replicates, and multiple-testing corrections addressed when relevant?
4. Clutter gate: Are routine details moved out of the main Results flow?
5. Claim-data gate: Does every conclusion stay within the data type and model system?

If any gate fails, revise the Results text before returning it. Do not return a known-overstated version as the final rewrite.

## Output Format

Prefer this format unless the user asks otherwise:

1. `Rewritten Results`: polished subsection text.
2. `Audit Notes`: short bullet list of the major fixes and any remaining data gaps.
3. `Suggested Title`: only if the original title overclaims or lacks focus.

Keep the final text publication-style, not explanatory. Put process comments in the audit notes, not inside the rewritten Results.
