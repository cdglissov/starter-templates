---
name: update-template
description: Updates dependencies for the template. Use when user asks to update template dependencies.
---

Find the dependencies in pyproject.toml and GitHub Actions workflows then update the dependencies to latest version. Make sure to also update the documentation in README.md to reflect any changes in the dependencies or usage instructions. Use the correct dependency management tool (the default is `uv`) to update the dependencies and ensure that the lockfile is updated accordingly.

Pre-commits are updated via `uv run pre-commit autoupdate`.
