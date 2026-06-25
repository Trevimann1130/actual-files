# Methodology

## Core Idea

DyNaBe is structured as a layered analysis:

1. a small confirmatory core for the main claim,
2. broader outcome and mechanism blocks for the applied questions,
3. a visible archive for older exploratory work.

## Outcome Logic

There are three central outcomes:

- `comfort_vote`: subjective thermal comfort
- `acceptance_vote` / `acceptance_num`: acceptability of the condition, relevant for flexible buildings
- `temperature_vote` / `temperature_num`: warm-cold sensation

## Analysis Blocks

### 1. Confirmatory Core

Script: [`../scripts/run_confirmatory_analysis.py`](../scripts/run_confirmatory_analysis.py)

Purpose:

- compare `pmv_7730` and `pmv_athb`
- use leave-one-person-out validation for new-person generalization
- run a small predefined HR marker extension
- test simple future-within-person personalization

Why this block exists:

- the main claim should not disappear inside a large model search
- the default path should stay readable for analysts and domain experts

### 2. Ordinal Cross-Checks

Script: [`../scripts/run_ordinal_models.py`](../scripts/run_ordinal_models.py)

Purpose:

- check whether the result pattern still holds when ordinal scales are treated as ordinal

### 3. Extended Multilevel Blocks

Script: [`../scripts/run_extended_multilevel_blocks.py`](../scripts/run_extended_multilevel_blocks.py)

Purpose:

- build the canonical HR-rich working dataset
- create lag variables such as `comfort_lag1`
- prepare dynamic and within/between-person blocks

### 4. Physiology Hypothesis Block

Script: [`../scripts/run_physio_hypothesis_suite.py`](../scripts/run_physio_hypothesis_suite.py)

Purpose:

- directly answer the nonlinear HRV questions from the email exchange
- test `SD1`, `SD2`, entropy measures, and reference markers one at a time
- compare every marker against the same baseline on the same subset

### 5. Advanced Suite

Script: [`../scripts/run_advanced_multilevel_suite.py`](../scripts/run_advanced_multilevel_suite.py)

Purpose:

- broaden the analysis to acceptance, temperature, profiles, nonlinearity, and robustness

## Primary vs Secondary

### Primary

- `pmv_7730` vs `pmv_athb` for `comfort_vote`
- generalization to new persons

### Secondary

- acceptance
- temperature
- dynamic / alliesthesia-like patterns
- physiologic markers

### Exploratory

- typologies
- older alternative paths
- historical plotting experiments

## Practical Rule

If a result is shown prominently in a presentation or publication, it should:

- be produced by the canonical script path,
- land in a documented output folder,
- and be mapped to a domain question in [`QUESTION_MATRIX.md`](QUESTION_MATRIX.md).
