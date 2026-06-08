---
name: nature-abstract-skills
description: Write, rewrite, polish, and audit Nature/Science-style abstracts for biomedical, life-science, physical-science, engineering, or interdisciplinary manuscripts. Use when Codex is asked to improve an Abstract from study findings, Results summaries, full manuscript sections, figure data, or rough notes; enforce a 125-150 word target when requested, the six-sentence abstract storyline, hard-data evidence, stand-alone readability, defined abbreviations, concise active language, calibrated significance, and iterative self-review until the abstract is data-bounded and publication-ready.
---

# Nature Abstract Skills

## Core Workflow

Use this skill to compress a manuscript into a stand-alone, high-impact abstract with a complete micro-story.

Follow this sequence:

1. Extract the background, gap, approach, key quantitative finding, mechanism, and significance from the user's material.
2. Draft a six-sentence abstract unless the target journal or user requests another format.
3. Keep the default target at 125 to 150 English words for Science-style abstracts.
4. Remove figure references, citations, undefined abbreviations, methods trivia, hype, and filler.
5. Audit the abstract with the Abstract review rubric.
6. Revise again if any audit gate fails, then return the final version with word count and audit notes.

For detailed audit criteria, read `references/abstract-rubric.md`.

## Input Handling

When the user provides Results, figures, or manuscript sections, treat them as the evidence boundary. Do not add data, mechanisms, clinical implications, or broad claims that are not supported.

When quantitative values are available, prioritize the few numbers that best prove the central claim. When key numbers are missing, write a conservative abstract and flag the missing hard data.

When the user provides only rough notes, first infer the safest claim level and identify missing items: model system, primary result, quantitative endpoint, mechanism, significance, and word limit.

## Six-Sentence Storyline

Use this default structure:

1. Background: broad scientific context or current state.
2. Problem/Gap: unresolved bottleneck or question, often beginning with `However`.
3. Approach: the central strategy, model, technology, or conceptual move.
4. Key finding: the strongest result, preferably with hard numbers.
5. Mechanism: the causal, biological, physical, chemical, or computational explanation.
6. Significance: the broader, data-bounded implication.

Allow sentence 4 to split into two sentences only when the key finding requires two linked quantitative results. If the word limit is strict, preserve the six functions even if sentence count changes slightly.

## Word Limit And Stand-Alone Rules

Default target: 125 to 150 words for Science-style abstracts.

Never include:

- Figure calls such as `Fig. 1` or `as shown`.
- References or citation numbers.
- Undefined abbreviations, except universally recognized terms such as DNA, RNA, or CPU.
- Routine protocol details, reagent amounts, centrifugation settings, catalog numbers, or supplement-level methods.
- Subjective hype such as `very interesting`, `astonishing`, `groundbreaking`, or `revolutionary`.

If the user requests a journal with a different limit, follow that limit and report the final word count.

## Language Rules

Make the abstract concise, active, and forceful.

- Use present tense for background and broad significance.
- Use past tense for completed experiments and findings when describing the authors' work.
- Prefer strong verbs: `uncover`, `resolve`, `redefine`, `accelerate`, `establish`, `reveal`, `identify`, `demonstrate`, `nominate`.
- Replace weak or vague claims with concrete evidence.
- Avoid opening with empty commonplaces such as `Cancer is a major threat to human health`.

## Evidence Calibration

Match claim strength to evidence.

- Use `demonstrated` or `established` only for directly tested findings.
- Use `suggested`, `nominated`, or `linked` for associative, cohort-level, enrichment, or discovery analyses.
- Use clinical claims only when clinical evidence is present.
- Use mechanistic claims only when mechanism data are provided.
- Use generalizable framework language only when the data support a broader principle beyond one narrow case.

## Hard Data Rules

The abstract should include hard data when available:

- effect size, percentage, fold change, hazard ratio, odds ratio, confidence interval, or benchmark;
- sample size, cohort size, or validation set when central;
- time, durability, efficiency, survival, response rate, or other field-specific endpoint;
- statistical correction only when it is central and compact.

Do not overload the abstract with secondary numbers. One or two decisive metrics are usually stronger than a list.

## Audit-And-Revise Loop

After the first draft, review it against these gates:

1. Sniff-test gate: Do the first two sentences show broad importance and a real frontier gap?
2. Hard-data gate: Does the core finding include quantitative or decisive evidence when available?
3. Micro-storyline gate: Do background, gap, approach, finding, mechanism, and significance connect causally?
4. General-reader gate: Is the abstract stand-alone, acronym-light, and readable by non-specialist scientists?
5. Hype gate: Is the final significance ambitious but bounded by the actual evidence?

If any gate fails, revise before returning the final abstract. Do not return a version that knowingly exceeds the evidence, word limit, or stand-alone requirements.

## Output Format

Prefer this format unless the user asks otherwise:

1. `Rewritten Abstract`: final abstract text.
2. `Word Count`: exact English word count when the abstract is in English.
3. `Audit Notes`: short bullet list of major fixes and remaining caveats.

Keep the abstract itself publication-style. Put process comments in the audit notes, not inside the abstract.
