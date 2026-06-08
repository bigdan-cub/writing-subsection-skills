---
name: nature-methods-skills
description: Rewrite, structure, and audit Nature/Science-style Methods sections for biomedical, life-science, computational, engineering, or interdisciplinary manuscripts. Use when Codex is asked to improve Methods text from rough protocols, manuscript drafts, Results-linked experiments, clinical cohorts, animal studies, cell assays, omics workflows, machine-learning pipelines, statistics sections, or data/code availability statements; enforce reproducibility, Results-mapped subheadings, key parameters, material provenance, ethics, controls, transparent data processing, statistical rigor, software versions, and iterative self-review until the Methods can support the manuscript claims.
---

# Nature Methods Skills

## Core Workflow

Use this skill to turn incomplete or narrative Methods text into a reproducible, audit-ready Methods section.

Follow this sequence:

1. Map each Results claim, figure, assay, cohort, model, or analysis to a corresponding Methods subsection.
2. Reorder Methods by the Results logic and experimental workflow: model/materials, intervention, data acquisition, data processing, statistics, and availability.
3. Add or request missing reproducibility details: source, catalog number, validation, parameters, controls, sample size, software, versions, and exclusion rules.
4. Calibrate Methods strength against claims: association methods cannot support causal conclusions; in vitro methods cannot support in vivo claims.
5. Audit the rewrite with the Methods review rubric.
6. Revise again if any audit gate fails, then return the final Methods text plus missing-information notes.

For detailed audit criteria, read `references/methods-rubric.md`.

## Input Handling

When the user provides Results or figure labels, build Methods subheadings that let readers locate the procedure behind each major result.

When the user provides rough protocol notes, preserve scientifically important parameters and remove SOP-level trivia that does not affect reproducibility.

When critical details are absent, do not invent them. Insert clear placeholders such as `[catalog number]`, `[IRB approval number]`, `[software version]`, `[power analysis method]`, or `[outlier rule]`, and list them in audit notes.

## Structure Rules

Use concise subheadings. Order them to mirror Results whenever possible.

Default biomedical order:

1. Study design, ethics, and sample inclusion.
2. Clinical cohort, animal model, cell line, organism, material, or dataset source.
3. Interventions, treatments, perturbations, or experimental procedures.
4. Data acquisition assays and instrumentation.
5. Data processing, normalization, quality control, and feature engineering.
6. Statistical analysis.
7. Data and code availability.

For computational or machine-learning studies, include dataset source, preprocessing, feature engineering, train/validation/test split, model architecture, hyperparameters, evaluation metrics, baseline comparators, software versions, and code availability.

## Reproducibility Detail Standard

Include details that determine whether a qualified peer can reproduce the result:

- Cell lines: source, catalog or accession, authentication such as STR profiling, mycoplasma testing, passage range when relevant, culture medium, supplements, temperature, atmosphere, and treatment conditions.
- Animals: species, strain, supplier, age, sex, housing, randomization, blinding, group allocation, humane endpoints, and ethics approval.
- Human samples: cohort source, inclusion/exclusion criteria, consent, IRB approval, clinical variables, biospecimen handling, and de-identification.
- Reagents and antibodies: supplier, catalog number, clone, dilution, lot when relevant, RRID when available, and validation method for key antibodies.
- Instruments and assays: instrument model, acquisition settings that affect results, calibration, thresholds, and quality-control rules.
- Sequencing and omics: library preparation, platform, depth, alignment or processing pipeline, genome/reference version, normalization, batch correction, and multiple-testing correction.
- Custom methods or algorithms: step-by-step workflow, hyperparameters, random seeds, training procedure, model selection, and repository or DOI.

Avoid citation nesting. If a standard method is cited, state the exact modification used in this study.

## Controls And Design

State controls and design safeguards when relevant:

- negative controls: vehicle, mock, untreated, scramble, isotype, empty vector, wild-type, sham, or no-template controls;
- positive controls: known inducer, inhibitor, benchmark model, validated marker, reference material, or standard dataset;
- design safeguards: randomization, blinding, blocking, counterbalancing, batch balancing, matched controls, and confounder adjustment.

If controls are absent or unclear, flag the gap. Do not imply a control existed if it was not provided.

## Data Processing And Statistics

Make the data pipeline explicit:

- how raw data became processed data;
- normalization and transformation choices;
- missing-value handling;
- outlier definition and whether rules were set before analysis;
- exclusion criteria;
- batch correction or confounder adjustment;
- number of biological and technical replicates;
- exact statistical test, sidedness, pairing, variance assumption, normality check, and correction for multiple comparisons;
- software, package, and version used for analysis and visualization.

Do not write only `standard statistical tests were used`. Use precise statements such as `Differences between two independent groups were evaluated with two-sided unpaired Welch's t-tests to account for unequal variances`.

## Data And Code Availability

End with a Data and Code Availability subsection when the study uses datasets, custom scripts, computational models, or trained algorithms.

Include:

- repository name and link or DOI when available;
- accession numbers for sequencing, proteomics, imaging, or clinical datasets;
- license or access restrictions when relevant;
- whether processed data, raw data, trained models, and scripts are available.

If code or data are unavailable, state the reason and avoid black-box claims.

## Claim-Method Fit

Check whether the method can support the manuscript's claims.

- Observational cohorts and correlation analyses support association, not direct causality.
- In vitro assays support cellular effects, not organism-level mechanism or clinical efficacy.
- Animal models support model-specific in vivo findings, not proof in humans.
- Machine-learning models require independent validation and meaningful baselines before strong predictive claims.
- Mechanistic claims require perturbation, temporal evidence, rescue, biochemical validation, or equivalent support.

## Audit-And-Revise Loop

After the first rewrite, review it against these gates:

1. Methodological-fit gate: Do the methods match the scientific claims?
2. Data-pipeline gate: Can raw data processing be reconstructed?
3. Controls gate: Are positive, negative, and baseline controls stated or flagged?
4. Statistical-power gate: Are sample size, replicate structure, tests, assumptions, and correction methods explicit?
5. Red-line gate: Are black-box algorithms, hidden code, p-hacking risks, unvalidated models/materials, or causality overreach present?

If any gate fails, revise the Methods or explicitly list the missing information before returning the final answer.

## Output Format

Prefer this format unless the user asks otherwise:

1. `Rewritten Methods`: structured manuscript-ready Methods text.
2. `Missing Information`: concise list of placeholders or details the user must supply.
3. `Audit Notes`: short list of claim-method fit issues, controls, statistics, and reproducibility risks.

Keep the Methods text practical and reproducible. Put uncertainty and requests for missing details in the notes, not hidden inside polished prose.
