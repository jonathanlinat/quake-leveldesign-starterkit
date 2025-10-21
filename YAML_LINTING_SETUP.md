# `YAML` Linting Setup Guide

This guide sets up automated `YAML` linting and formatting using `pre-commit` hooks.

Once configured, `YAML` files will be automatically checked and fixed on every commit, ensuring consistent formatting, proper indentation, and catching syntax errors before they reach the repository.

---

## Install `pre-commit`

### Windows

```powershell
# Using pip (works in PowerShell or CMD)
pip install pre-commit

# Or using Chocolatey
choco install pre-commit

# Or using Scoop
scoop install pre-commit
```

### Linux (Ubuntu)

```bash
# Using pip
pip install --user pre-commit

# Or using apt
sudo apt install pre-commit
```

### macOS

```bash
# Using Homebrew
brew install pre-commit

# Or using pip
pip install pre-commit
```

---

## Set Up the Hooks

```bash
pre-commit install
```

---

## Run the Checks

```bash
# Run on all files
pre-commit run --all-files

# Or commit to trigger automatically
git commit -m "test"
```

---

## What This Does

The `pre-commit` hook will automatically:

- [x] Check `YAML` syntax validity
- [x] Fix indentation (2 spaces consistently)
- [x] Remove trailing whitespace
- [x] Ensure files end with a newline
- [x] Fix line endings (LF)
- [x] Lint for common `YAML` issues

> [!NOTE]
> `yamlfmt` configuration is in the `.yamlfmt` file.

---

## Additional Commands

```bash
# Run on all files
pre-commit run --all-files

# Run on specific files
pre-commit run --files .github/workflows/*.yml

# Run a specific hook
pre-commit run yamllint --all-files

# Skip hooks (emergency only)
git commit --no-verify -m "skip hooks"
```
