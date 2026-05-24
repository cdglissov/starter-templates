# Python Copier Template

Copier template for quickly creating a modern Python repository.

## Usage

Install Copier, then generate a project:

```sh
uvx copier copy gh:cdglissov/starter-templates my-project
```

For local testing from this repository:

```sh
uvx copier copy . /tmp/my-project
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
