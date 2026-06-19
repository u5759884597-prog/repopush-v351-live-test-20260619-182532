# Quickstart

Complete these steps to verify the main workflow.

## Install

```bash
pip install repopush
python src/repopush.py audit --input sample_product_brief.json
```

## Steps

1. Create a product brief JSON file.
2. Run `python src/repopush.py compile --input sample_product_brief.json --platform github --out output_pack`.
3. Run `python src/repopush.py validate --pack output_pack/github`.
4. Run a dry-run install plan before opening a PR.

## Expected result

You should have a working local setup and a clear path to examples in docs/EXAMPLES.md.
