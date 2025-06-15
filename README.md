![Python 3.12+](https://img.shields.io/badge/python-3.12+-blue.svg)
![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen.svg)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

# Your Project

## Local development

### 1. Install tooling

```commandline
pip install -U uv
```

### 2. Install dependencies

```commandline
uv sync
```

### 3. Enable Git hooks

```commandline
pre-commit install
pre-commit install --hook-type commit-msg
pre-commit autoupdate
```

### 4. Running hooks manually

```commandline
pre-commit run --all-files
```

### 5. Running tests

```commandline
pytest -vv --junitxml=report.xml --cov=app --cov-report=xml --cov-report=term
```

## Using this template for your own project

1. **Reset version to `0.0.0`.**
   Update the following files so the Release Please starts versioning from scratch:

   * `.release-please-manifest.json`
   * `pyproject.toml`

2. **Clean the changelog.**
   Remove everything in `CHANGELOG.md`.

3. Replace placeholder metadata (`project_name`, author name, description) wherever it appears.

That is all, you can now commit and start normal Release Please driven versioning.
