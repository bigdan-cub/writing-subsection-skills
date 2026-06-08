# Methods Review Rubric

Use this rubric after drafting or rewriting a Methods section.

## Methodological Fit Test

Pass criteria:

- Each major claim in Results, Abstract, Introduction, or Discussion has an appropriate method.
- Causal claims are supported by perturbation, rescue, temporal, randomized, or mechanistic designs.
- In vivo and clinical claims are not supported only by in vitro assays.
- Computational claims use suitable models, baselines, validation, and evaluation metrics.

Failure response:

- Downgrade the claim or flag the missing method.
- Add the missing control, validation, or model-system limitation.

## Data Pipeline Transparency Test

Pass criteria:

- The path from raw data to final figure is reconstructable.
- Missing-value handling is stated.
- Outlier rules are explicit and not post hoc.
- Feature engineering, normalization, transformations, thresholds, and batch correction are described.
- Software packages and versions are listed.

Failure response:

- Add placeholders for missing processing steps.
- Replace vague statements such as `data were cleaned` with explicit rules.

## Rigorous Controls Test

Pass criteria:

- Negative controls are listed where needed.
- Positive controls or benchmark baselines are listed where needed.
- Randomization, blinding, matching, or confounder adjustment is described for complex systems.
- Controls map to the assays or models they validate.

Failure response:

- Flag missing controls as a reproducibility or interpretation risk.
- Do not imply controls were performed unless provided.

## Statistical Power And Rigor Test

Pass criteria:

- Sample sizes and replicate types are clear.
- Sample-size determination or power analysis is stated when relevant.
- Statistical tests include sidedness, pairing, variance assumption, and normality assessment when applicable.
- Multiple-testing correction is stated for high-throughput analyses.
- Exact software and visualization tools are named with versions.

Failure response:

- Add missing statistical placeholders.
- Replace generic `t-test` or `ANOVA` descriptions with complete test specifications.

## Material And Model Validation Test

Pass criteria:

- Cell lines include source, authentication, and mycoplasma status.
- Animals include strain, age, sex, housing, allocation, and ethics approval.
- Human studies include IRB approval, consent, inclusion/exclusion criteria, and sample handling.
- Antibodies and key reagents include supplier, catalog number, RRID when available, and validation method.
- Custom materials, algorithms, or models include enough detail to reproduce.

Failure response:

- Add placeholders for provenance and validation.
- Flag unvalidated foundations as high-risk.

## Black Box And Availability Test

Pass criteria:

- Custom scripts, machine-learning models, and analysis pipelines are available or fully described.
- Hyperparameters, random seeds, train/test splits, evaluation metrics, and baselines are stated when relevant.
- Data and Code Availability statements provide links, DOI, accession numbers, or justified restrictions.

Failure response:

- Request repository, DOI, accession number, or complete algorithm details.
- Mark `in-house algorithm` language as unacceptable unless reproducible details are supplied.

## P-Hacking And Data Dredging Test

Pass criteria:

- Exclusion and outlier rules are pre-specified or transparently justified.
- Statistical tests are chosen based on design and assumptions, not significance outcome.
- Exploratory and confirmatory analyses are distinguished.

Failure response:

- State the risk explicitly.
- Require pre-specified exclusion rules and confirmatory validation.

## Final Acceptance Standard

Accept the Methods only if:

- A qualified peer could reproduce the major experiments or analyses.
- Materials, models, ethics, controls, and statistics are transparent.
- Data and code availability is adequate for the evidence type.
- The methods can support the manuscript's claim level.
