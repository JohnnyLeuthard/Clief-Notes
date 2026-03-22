# Stage: Compliance Parsing

**Job**: Analyze the retrieved CSV data against vault naming standards to identify non-compliant accounts.

## Inputs

- **Layer 4 (Working)**: `../02_data_fetch/output/vault_data.csv` — Raw data from the previous stage.
- **Layer 3 (Reference)**: `../../references/naming_standards.md` — Organization naming conventions to check against.

## Process

1. Load the CSV data from Stage 02's output.
2. Parse each row, extracting account names and relevant metadata fields.
3. Compare each account against the naming rules defined in `naming_standards.md`.
4. Flag any accounts that do not comply, noting the specific rule violation.
5. Generate a compliance summary report.

## Outputs

- `compliance_report.md` → `output/compliance_report.md`

## Review Gate

Stop here. The human reviews the compliance report. Non-compliant accounts identified here may become inputs for the `psPAS` remediation pipeline at `../../psPAS/CONTEXT.md`.
