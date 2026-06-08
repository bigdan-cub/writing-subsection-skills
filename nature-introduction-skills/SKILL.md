---
name: nature-introduction-skills
description: Rewrite, polish, and audit biomedical or life-science manuscript Introduction sections in a Nature/Science style. Use when Codex is asked to improve Introduction text from manuscript drafts, study findings, Results summaries, figure promises, background notes, or citation plans; enforce the four-paragraph funnel structure, broad non-specialist opening, authentic knowledge gap, original approach, payoff/signpost ending, concise active language, fair citation framing, and iterative self-review until the Introduction promise matches the Results evidence.
---

# Nature Introduction Skills

## Core Workflow

Use this skill to turn a draft Introduction into a compact, high-momentum, general-science argument that leads cleanly into the Results.

Follow this sequence:

1. Extract the field-level problem, known knowledge, true unresolved gap, study approach, central finding, and Results-supported payoff.
2. Rewrite the Introduction with the four-part funnel structure.
3. Remove jargon, overlong literature-review material, inflated promises, and unsupported novelty claims.
4. Audit the rewrite with the Introduction review rubric.
5. Revise again if any audit gate fails.
6. Return the final Introduction plus concise audit notes and any unresolved evidence or citation gaps.

For detailed audit criteria, read `references/introduction-rubric.md`.

## Input Handling

When the user provides Results text, figure summaries, or study findings, treat them as the evidence boundary for the Introduction's final promise. Do not promise a mechanism, clinical relevance, universality, or conceptual solution that the Results do not support.

When the user provides only background notes, identify what is missing before drafting: study question, central finding, key method, model system, gap, and target journal tone.

When citations are requested but not provided, use citation slots such as `[key citation]` rather than inventing sources.

## Funnel Structure

Write the Introduction as 3 to 4 compact paragraphs, usually 400 to 600 words unless the user requests another length.

Use this sequence:

1. Big picture: open with a broad scientific or biomedical problem that non-specialist scientists can understand.
2. Knowledge gap: summarize what is known, then define the unresolved question, contradiction, or bottleneck.
3. Approach and hypothesis: explain the study's original angle, method, hypothesis, cohort, model, or experimental strategy.
4. Payoff and signpost: preview the central finding and its significance in a way that points naturally to the first Results figure.

Do not write a full literature review. Include only the field context needed to make the gap feel real and consequential.

## Paragraph Goals

Big picture paragraph:

- Start from disease burden, scientific mystery, technological barrier, ecological relevance, or conceptual importance.
- Avoid opening with narrow molecules, obscure pathways, niche techniques, or unexplained abbreviations.
- Answer why a scientist outside the field should care.

Knowledge gap paragraph:

- Respect prior work before defining what remains unresolved.
- Use sharp gap language: `However, despite these advances...`, `A central question remains...`, or `The mechanism underlying... remains unclear`.
- Avoid low-value gaps such as only testing a known factor in another cancer or repeating a known assay with a newer instrument unless the new setting changes the underlying concept.

Approach paragraph:

- State why this study could resolve the gap: new model, longitudinal design, perturbation, clinical cohort, multi-omics integration, structural method, causal test, or conceptual reframing.
- Use active voice where appropriate: `Here we...`, `We combined...`, `We tested...`.
- Define specialized terms and abbreviations at first use.

Payoff paragraph:

- Give a direct preview of the main discovery.
- Keep the promise matched to the Results.
- End by pointing toward the logic of the Results rather than using vague phrases such as `we discuss the implications`.

## Language Rules

Make the Introduction concise, precise, and story-driven.

- Prefer active constructions: `We demonstrate`, `We identify`, `We test`.
- Use precise verbs: `elucidate`, `resolve`, `harness`, `diverge`, `converge`, `nominate`, `reveal`, `establish`.
- Remove filler such as `in recent years`, `more and more attention`, `it is well known`, and broad unsupported claims.
- Define necessary jargon once, then use it consistently.
- Avoid attacking prior work. Frame the study as extending, resolving, or testing an unresolved issue.

## Promise Calibration

Match the final paragraph to the Results evidence.

- If the Results are observational, promise association, stratification, or candidate nomination.
- If the Results include perturbation and rescue, promise causal or mechanistic insight only within the tested model.
- If the Results are preclinical, avoid claiming human efficacy.
- If the Results are single-cohort or single-model, avoid universal language.
- If the paper does not resolve a long-standing debate, do not claim that it does.

## Citation Framing

Use citations to map the field honestly and efficiently.

- Cite foundational work, recent high-impact advances, and key conflicting evidence when relevant.
- Avoid citation clustering that is mostly self-citation.
- Do not omit major opposing studies if the gap depends on a controversy.
- Keep references attached to specific knowledge claims, not generic background decoration.

## Audit-And-Revise Loop

After the first rewrite, review it against these gates:

1. General-science gate: Can a non-specialist scientist understand the first paragraph and why the problem matters?
2. Gap-authenticity gate: Is the knowledge gap real, consequential, and more than a narrow incremental slot?
3. Over-promising gate: Does the final promise match the actual Results and evidence type?
4. Citation-sincerity gate: Is the field context fair, current, and not self-serving?
5. Narrative-momentum gate: Does each paragraph narrow the focus smoothly and make the next paragraph feel necessary?

If any gate fails, revise before returning the final version. Do not return an Introduction that knowingly overstates novelty, causality, generality, or translational impact.

## Output Format

Prefer this format unless the user asks otherwise:

1. `Rewritten Introduction`: polished Introduction text.
2. `Audit Notes`: short bullet list of major fixes and remaining caveats.
3. `Suggested Opening/Closing`: optional alternative first or last sentence if the draft needs stronger narrative focus.

Keep the rewritten Introduction manuscript-style. Put explanations about editing choices in the audit notes, not inside the manuscript text.
