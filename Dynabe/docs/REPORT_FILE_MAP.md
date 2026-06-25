# Report File Map

This note maps the stakeholder report to the files in this reduced export.

## Final document

- `analysis/stakeholder_report/DyNaBe_Auswertungsbericht_Stakeholder.docx`
- built by `scripts/build_word_report.py`

## Main prepared datasets

- `analysis/all_core_dataset.csv`
  - merged comfort dataset across all source groups
  - used for overall comfort correlations, aggregated comfort models, and person-feature checks

- `analysis/all_core_dataset_summary.json`
  - counts and overview numbers for the data basis section

- `analysis/extended_blocks/extended_hr_dataset.csv`
  - HR-rich working dataset
  - used for dynamic tables and HR-related sections

## Report tables and summary blocks

- `analysis/confirmatory/primary_model_delta.csv`
  - used for the LOPO comparison between PMV 7730 and ATHB

- `analysis/confirmatory/hr_marker_comparison.csv`
  - used for the report section on added value of BPM, RMSSD, and SNS

- `analysis/confirmatory/primary_person_metrics.csv`
  - used to build the person-level comparison figure

- `analysis/physio_hypotheses/physio_comfort_hypothesis_comparison.csv`
  - used for the nonlinear HRV section, especially ApEn, SD1, and SD2

- `analysis/advanced_suite/ordinal_mixed/ordinal_mixed_comparison.csv`
  - used for person-adjusted comparisons for comfort, temperature, and acceptance

- `analysis/extended_blocks/lag_effect_comparison.csv`
  - used for the dynamic and lag-based comfort section

- `analysis/advanced_suite/feature_stability/feature_stability_summary.csv`
  - used for the parameter-importance section

- `analysis/advanced_suite/profiles/individual_reaction_profiles.csv`
  - used for the person-level dynamic summary

- `analysis/advanced_suite/nonlinearity/nonlinearity_comparison.csv`
  - used for the dynamic/nonlinear figure

## Figure inputs and outputs

- `analysis/ordinal_models/comfort_hr_ordinal_fair_comparison.csv`
  - used by `scripts/run_final_paper_figures.py` for the ordinal HR panel

- `analysis/paper_plots/final_figures/figure1_person_level_model_comparison.png`
  - included in the report as the person-level model comparison figure

- `analysis/paper_plots/final_figures/figure2_hr_added_value.png`
  - included in the report as the HR added-value figure

## Suggested files to inspect first

- `scripts/prepare_all_core_dataset.py`
- `scripts/run_extended_multilevel_blocks.py`
- `scripts/run_confirmatory_analysis.py`
- `scripts/run_physio_hypothesis_suite.py`
- `scripts/run_advanced_multilevel_suite.py`
- `scripts/run_final_paper_figures.py`
- `scripts/build_word_report.py`
