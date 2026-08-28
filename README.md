# etlpocket

Reusable ETL skeleton for the CSVs I get at work

## Install

```bash
pip install -r requirements.txt
```

## How to use

```bash
python pipeline.py raw.csv --config config.yaml --out clean.csv
```

## Features

- Config-driven column renames and type casts
- Drops duplicates, trims strings, normalizes dates
- Writes a cleaning report next to the output
- Chunked reading for files that do not fit in memory

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── config.yaml
├── pipeline.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
