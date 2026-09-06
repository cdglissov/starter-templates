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
## Generated Python Project

After generation:

```sh
cd my-project
make bootstrap
make check
```

This creates the lockfile, installs dependencies, initializes a Git repository if needed, generates docs, and installs pre-commit hooks and their environments.

Optionally install [apm](https://microsoft.github.io/apm/getting-started/installation/)

Finally, use the attached skills to update the template or tailor it to your use.

# TODOs:

- Refine current templates
    - Significantly improve doc generation
    - Add improved workflows
    - Add standardized dockerfile with multistaging and debian base image
- Add better telemetry out of the box (Cookiecutter OTEL collector)
