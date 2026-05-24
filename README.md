# Python Copier Template

Copier template for quickly creating a modern Python repository.

## Usage

Install Copier, then generate a project:

```sh
uvx copier copy gh:cdglissov/python-template my-project
```

For local testing from this repository:

```sh
uvx copier copy . /tmp/my-project
```

Updating your project:

```sh
uvx copier update --defaults
```

Code coverage is reported directly in pytest output, both locally and in CI. No external coverage service or repository token is required.

The generated project uses:

- `src/` package layout
- `uv` for project and dependency management
- `.python-version` for interpreter selection
- Ruff for linting and formatting
- Pyrefly for type checking
- pytest, pytest-cov, and coverage.py for tests and coverage reports
- MkDocs Material for fast documentation generation
- pre-commit hooks
- GitHub Actions CI and Dependabot
- GitHub issue and pull request templates
- a basic security policy

## Generated Project

After generation:

```sh
cd my-project
make bootstrap
make check
make docs
```

This creates the lockfile, installs dependencies, initializes a Git repository if needed, generates docs, and installs pre-commit hooks and their environments.
