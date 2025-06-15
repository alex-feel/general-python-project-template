You can run the following commands to additionally check code:

1. `uv run pre-commit run --all-files` — to run pre-commit hooks, including ruff.

2. `uv run pytest -vv --junitxml=report.xml --cov=app --cov-report=xml --cov-report=term` — to run tests. After you can check `report.xml` and `coverage.xml` files to get information about test results and test coverage.
