# CyberArk Vault Automation Workspace

You are in the root of a CyberArk operations workspace. This workspace uses the Model Workspace Protocol (MWP) — a layered context hierarchy where folder structure replaces framework-level orchestration.

## How to Navigate

Read `CONTEXT.md` in this directory to route the user's request to the correct sub-workspace. Do not load files from sub-workspaces until you have routed.

## Protocol Rules

- **Layered loading**: Only read the CONTEXT.md for the stage you are currently in. Do not preload files from other stages.
- **Review gates**: Every stage ends with a stop. Wait for explicit human approval before proceeding to the next stage.
- **Plain text interface**: All stage communication happens through markdown and CSV files in `output/` folders.
- **No simulated data**: Never generate fake vault data, sample CSVs, or mock query results. Use pipeline-specific scripts (e.g., `EVD/scripts/`) for all mechanical execution.
- **No inline execution code**: When a script is needed, reference the appropriate file in the pipeline's scripts directory. Do not generate PowerShell or Python inline.
- **Self-contained pipelines**: Each pipeline (EVD, psPAS) carries its own references in its `references/` folder. Do not duplicate reference material into stage-level files — point to the pipeline's `references/` instead. The `_config/` folder holds only cross-pipeline pointers.
