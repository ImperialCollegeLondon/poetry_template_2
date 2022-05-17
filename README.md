# Poetry Template

[![Test and build](https://github.com/ImperialCollegeLondon/poetry_template_2/actions/workflows/ci.yml/badge.svg)](https://github.com/ImperialCollegeLondon/poetry_template_2/actions/workflows/ci.yml)

This is a minimal Python 3.9 application that uses [poetry](https://python-poetry.org) for packaging and dependency management. It also provides [pre-commit](https://pre-commit.com/) hooks (for [Black](https://black.readthedocs.io/en/stable/) and [Flake8](https://flake8.pycqa.org/en/latest/)) and automated tests using [pytest](https://pytest.org/) and [GitHub Actions](https://github.com/features/actions). Pre-commit hooks are automatically kept updated with a dedicated GitHub Action. It was developed by the [Imperial College Research Computing Service](https://www.imperial.ac.uk/admin-services/ict/self-service/research-support/rcs/).

To use this repository as a template for your own application:

1. [Download and install Poetry](https://python-poetry.org/docs/#installation) following the instructions for your OS.
1. Click the green "Use this template" button above
1. Name and create your repository
1. Clone your new repository and make it your working directory
1. Replace instances of `myproject` with your own application name. Edit:
   - `pyproject.toml`
   - `tests/test_myproject.py`
   - `setup.cfg`
   - Rename `myproject` directory
1. Set up the virtual environment:

   ```bash
   poetry install
   ```

1. Activate the virtual environment (alternatively, ensure any python-related command is preceded by `poetry run`):

   ```bash
   poetry shell
   ```

1. Install the git hooks:

   ```bash
   pre-commit install
   ```

1. Run the main app:

   ```bash
   python -m myproject
   ```

1. Run the tests:

   ```bash
   pytest
   ```
