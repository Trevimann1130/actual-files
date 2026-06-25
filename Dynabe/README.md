# DyNaBe Partner Export

This folder is a reduced DyNaBe export for project partners.

It contains only:

- the scripts needed to understand how the stakeholder report was assembled,
- the prepared analysis tables that feed the report,
- the two final figures used in the report,
- and the generated stakeholder report itself.

It deliberately does not contain older exploratory branches, archived scripts,
or raw source files that are not needed to follow the report logic.

## Reading order

1. `analysis/stakeholder_report/DyNaBe_Auswertungsbericht_Stakeholder.docx`
2. `docs/REPORT_FILE_MAP.md`
3. `docs/METHODOLOGY.md`
4. `scripts/build_word_report.py`

## Main structure

- `scripts/`: commented analysis and reporting scripts
- `analysis/`: reduced result files used by the report
- `docs/`: short orientation documents

## Practical note

The report is built from prepared analysis outputs. In other words, this export
is designed for transparency and explanation, not for rerunning the full
research pipeline from raw measurement files.
