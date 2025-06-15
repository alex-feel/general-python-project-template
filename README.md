[![Python 3.12+](https://img.shields.io/badge/python-3.12+-blue.svg)](https://www.python.org/)
[![uv](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/uv/main/assets/badge/v0.json)](https://github.com/astral-sh/uv)
[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen.svg)](https://github.com/pre-commit/pre-commit)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)

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
   Update the following files so Release Please starts versioning from scratch:

   * `.release-please-manifest.json`
   * `pyproject.toml`

2. **Clean the changelog.**
   Remove everything in `CHANGELOG.md`.

3. **Replace placeholder metadata.**
   Search for `project_name`, author name, description, etc., and update to match your project.

4. **Add GitHub tokens for Actions.**

   | Secret name | Token scopes (Fine-grained) | Purpose |
   |-------------|----------------------------|---------|
   | `PRE_COMMIT_TOKEN` | *Repository permissions* → **Contents** → **Read** | Allows the “Run Pre-Commit” workflow to fetch the repo and run hooks. |
   | `RELEASE_PLEASE_TOKEN` | *Repository permissions* → **Contents** → **Read & Write**<br>*Repository permissions* → **Pull requests** → **Read & Write** | Lets Release Please create release PRs, tags and update `uv.lock`. |

   **How to create and add a token**

   1. Go to **Settings → Developer settings → Personal access tokens → Fine-grained tokens**.
   2. Click **Generate new token**, select the repository, set the scopes above, generate and copy the token.
   3. Open **Repository → Settings → Secrets and variables → Actions**.
   4. Add each token under **Repository secrets** with the exact names `PRE_COMMIT_TOKEN` and `RELEASE_PLEASE_TOKEN`.

That’s all — commit your changes, push, and the GitHub Actions workflows will run out-of-the-box.
