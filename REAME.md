# New Repo

## Setup
### Create a Virtual Environment
```shell
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Install Dependencies
#### Production dependencies
```shell
pip install -r requirements.txt

```
#### Development dependencies (includes linting, formatting, testing)
```
pip install -r requirements.dev.txt

```

### Run Tests
```shell
pytest
```

### Format Code (Black)
```shell
black .
```

### Lint Code (Ruff)
```shell
ruff check .

```
### Run Pre-Commit Hooks
```shell
pre-commit run --all-files

```

## GitHub Actions (CI/CD)
This project includes a GitHub Actions workflow that automatically:
 - Runs pytest on Linux, Windows, and macOS
 - Uses pre-commit hooks to enforce code quality

Every push and pull request triggers these checks.
