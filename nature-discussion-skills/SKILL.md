---
name: nature-discussion-skills
description: Rewrite, polish, and audit biomedical or life-science manuscript Discussion sections in a Nature/Science style. Use when Codex is asked to improve Discussion text from Results, figure summaries, manuscript drafts, reviewer concerns, or study findings; enforce the hourglass Discussion structure, direct-answer opening, contextualization, mechanism interpretation, honest limitations, broad significance, conceptual conclusion, calibrated certainty, and iterative self-review until claims remain ambitious but data-bounded.
---

# Nature Discussion Skills

## Core Workflow

Use this skill to transform a Results-bound manuscript Discussion into a broad, rigorous, and intellectually honest scientific argument.

Follow this sequence:

1. Extract the study's core question, strongest Results-supported claim, model system, evidence level, and unresolved gaps.
2. Rewrite the Discussion with an hourglass structure: local discovery, mechanism/context, limitations, broad significance, conceptual outlook.
3. Calibrate certainty: state proven findings firmly and extended implications cautiously.
4. Audit the rewrite with the Discussion review rubric.
5. Revise again if any audit gate fails.
6. Return the final Discussion text plus concise audit notes and remaining caveats.

For detailed audit criteria, read `references/discussion-rubric.md`.

## Input Handling

When the user provides Results text, figures, or findings, treat those as the evidentiary boundary for the Discussion. Do not introduce claims that require unprovided experiments, clinical data, animal data, or mechanistic proof.

When the user provides only a rough finding list, first infer the safe claim level and mark missing context, such as model system, sample size, causal perturbation, clinical validation, opposing literature, or mechanism.

When the user provides contradictory or negative findings, integrate them into the Discussion rather than smoothing them away. Use conflict and boundary conditions to sharpen the scientific argument.

## Hourglass Structure

Write the Discussion from local discovery to global significance:

1. Direct answer: summarize the central finding in one compact opening paragraph.
2. Context and mechanism: place the finding against prior work, explain likely mechanisms, and address agreement or conflict.
3. Limitations and unexpected results: state meaningful technical, biological, or translational boundaries.
4. Significance: explain why the finding matters beyond the narrow assay or disease subtype.
5. Conceptual conclusion: close with a model, hypothesis, framework, or future route that follows from the data.

Do not turn the Discussion into a Results recap. Each paragraph should add interpretation, context, mechanism, limitation, or significance.

## Five-Pass Writing Method

Use these passes when rewriting:

- Direct answer: open with `In this study, we demonstrate that...` or an equivalent direct statement if the data support demonstration. Use `show`, `reveal`, or `suggest` when evidence is weaker.
- Contextualization and mechanics: compare with prior work, explain what is consistent, what is advanced, and why discrepancies may exist.
- Limitations: identify real boundaries and convert them into testable next steps.
- So what: broaden the implication for the field, adjacent disciplines, disease biology, therapeutic strategy, technology, or conceptual understanding.
- Conceptual conclusion: end with a restrained model or future research blueprint rather than a promotional claim.

## Certainty Calibration

Match language to evidence strength.

- Use firm language for directly demonstrated findings: `demonstrates`, `establishes`, `indicates`, `supports`.
- Use cautious language for inference: `suggests`, `implies`, `is consistent with`, `may`, `could`, `likely`.
- Use associative language for cohort, transcriptomic, enrichment, or observational results: `associated with`, `linked to`, `nominated`, `prioritized`.
- Use causal language only when perturbation, rescue, temporal design, or equivalent causal evidence supports it.

Do not write clinical cure, therapeutic transformation, universal mechanism, or field-wide replacement claims unless the provided evidence actually supports them.

## Context And Conflict

Discussion should engage the field, not just the authors' data.

- Name the type of prior evidence being extended, such as earlier association, phenotype, pathway, structure, model, or clinical observation.
- If prior work agrees, explain what the present study adds.
- If prior work conflicts, state the discrepancy respectfully and propose plausible reasons such as model system, species, disease stage, cell state, assay sensitivity, cohort composition, endpoint, or perturbation timing.
- Avoid dismissive language toward previous studies.

If the user asks for citations but does not provide sources, flag citation slots instead of inventing references.

## Limitations

Include limitations that materially affect interpretation:

- Model boundary: in vitro, mouse, organoid, retrospective cohort, single-center dataset, specific cell line, or specific disease subtype.
- Causal boundary: association without loss-of-function, gain-of-function, rescue, temporal order, or mechanism.
- Measurement boundary: bulk profiling, resolution limit, indirect assay, antibody specificity, detection threshold, or short follow-up.
- Translational boundary: lack of pharmacology, safety, dosing, human validation, prospective trial, or independent cohort.

Weak limitations such as `time was limited` or generic `larger studies are needed` are insufficient unless tied to a concrete scientific uncertainty.

## Broad Significance

Make the Discussion readable beyond a narrow specialist audience.

- Connect the local discovery to a broader problem: disease evolution, treatment resistance, immune regulation, developmental logic, systems biology, target discovery, patient stratification, or technology design.
- Explain why the finding changes how the field should think, classify, measure, or test the phenomenon.
- Keep significance proportional to the evidence.

## Audit-And-Revise Loop

After the first rewrite, review it against these gates:

1. Over-claiming gate: Does every major claim match the Results evidence and model system?
2. Intellectual-honesty gate: Does the Discussion address relevant opposing or unresolved evidence when available?
3. Limitation gate: Are limitations specific, consequential, and connected to future tests?
4. No-repetition gate: Does the text add interpretation rather than restating Results?
5. Broad-impact gate: Would a non-specialist scientist understand why the work matters?

If any gate fails, revise before returning the final version. Do not return a Discussion that knowingly exaggerates causality, clinical relevance, universality, or mechanistic certainty.

## Output Format

Prefer this format unless the user asks otherwise:

1. `Rewritten Discussion`: polished Discussion text.
2. `Audit Notes`: short bullet list of major fixes and remaining caveats.
3. `Suggested Conceptual Close`: optional final sentence or model statement if the existing ending is weak.

Keep the rewritten Discussion publication-style. Put explanations about editing choices in the audit notes, not inside the manuscript text.
