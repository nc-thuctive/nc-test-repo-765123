# CLAUDE.md

This file provides guidance for AI assistants working in this repository.

## Repository Overview

A minimal Python repository containing a single FizzBuzz implementation. It serves as a simple demonstration or test project with no external dependencies.

## Project Structure

```
nc-test-repo-765123/
├── CLAUDE.md        # This file
├── README.md        # Project readme
└── fizzbuzz.py      # FizzBuzz implementation
```

## Language & Runtime

- **Language**: Python 3 (no specific version pinned)
- **Dependencies**: None — standard library only
- **No virtual environment, package manager, or build system**

## Running the Code

```bash
python fizzbuzz.py
```

Prints numbers 1–100 with substitutions:
- Multiples of 15 → `FizzBuzz`
- Multiples of 3 → `Fizz`
- Multiples of 5 → `Buzz`
- All others → the number itself

## Development Conventions

- **Style**: Follow standard PEP 8 Python conventions
- **Logic order**: Check `% 15` before `% 3` and `% 5` to avoid shadowing the combined case
- **No imports**: Keep the file dependency-free unless a clear need arises

## Testing

There is no test suite configured. If adding tests:
- Use `pytest` (install via `pip install pytest`)
- Place tests in a `tests/` directory or in files named `test_*.py`
- Run with: `pytest`

## Linting & Formatting

No linting or formatting tools are configured. Recommended setup if needed:
- **Formatter**: `black fizzbuzz.py`
- **Linter**: `flake8 fizzbuzz.py`

## Git Workflow

- **Main branch**: `main`
- **Feature branches**: Use descriptive names, e.g. `claude/<feature-description>-<id>`
- Commit messages should be clear and imperative (e.g. `Add fizzbuzz program`)
- No CI/CD pipelines are configured

## Key Notes for AI Assistants

- This is a minimal repo — avoid over-engineering solutions
- There are no environment variables, secrets, or external services
- When adding features, keep the code simple and dependency-free unless explicitly asked otherwise
- If tests are requested, use `pytest` as the default framework
