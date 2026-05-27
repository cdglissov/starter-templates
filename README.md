# Python Copier Template (WIP)

Copier template for quickly creating a modern Python repository.

## Usage

Install Copier, then generate a project:

```sh
uvx copier copy gh:cdglissov/starter-templates my-project
```

Updating your project:

```sh
uvx copier update --defaults
```
## Generated Project

After generation:

```sh
cd my-project
make bootstrap
make check
make docs
```

This creates the lockfile, installs dependencies, initializes a Git repository if needed, generates docs, and installs pre-commit hooks and their environments.

# Todos:
- Create template for vscode workspace backend + frontend design
- Create template for monorepo (uv workspaces)
- Refine current templates
    - Significantly improve doc generation
    - Add improved workflows
    - Add standardized dockerfile with multistaging and debian base image
- Integrate praxis agent harness with project setup
- Simplify third parties
- Add better telemetry out of the box (OTEL/Improved native logging)