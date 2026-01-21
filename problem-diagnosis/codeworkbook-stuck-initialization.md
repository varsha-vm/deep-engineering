# Workbook Stuck in Initialization

## Symptom
- Code workbook failed to start

## Root cause
- Deprecated foundry_ml in meta.ml

## How we diagnosed
1. Checked runtime logs
2. Verified meta.ml
3. Compared with working workbook
4. Reviewed Palantir documentation for library / python version deprecation
5. Figured out library suffixed w/ foundry_ml are deprecated and palantir_model librabry to be used instead


## Fix
- Removed ML block
- Updated runtime
- Applyed the palantir_model changes with python upgrade to support compatibility of python w/ Palantir library
- Re-ran the code workbooks builds to ensure the working.

