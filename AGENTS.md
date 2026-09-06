# Repository Guide

This repo is a Copier template for bootstrapping Python projects with AI-friendly defaults. It supports Windows and Linux.

## Evaluation

Generate a project locally:

```bash
uvx copier copy . test-project
```

Then run checks inside `test-project`:

```bash
make bootstrap
make check
```

## Repository Layout

```text
.
|-- AGENTS.md                              # Template repo instructions
|-- README.md                              # Usage, contribution notes, and test flow
|-- copier.yml                             # Copier questions, defaults, validators
|-- .github/                               # Template-repo GitHub files
`-- python-project-template/               # Files rendered into generated Python projects
    |-- AGENTS.md.jinja
    |-- Makefile.jinja
    |-- pyproject.toml.jinja
    |-- README.md.jinja
    |-- agents/skills/
    |-- .github/
    |-- .vscode/
    |-- scripts/pre-commit-hooks/
    |-- src/{{ package_name }}/
    `-- tests/
```

## Validation outside the template

To run pre-commits and ruff you can use:
```bash
uvx prek run --all-files --config .pre-commit-config.yaml
uvx ruff check . --fix
uvx ruff format .
```