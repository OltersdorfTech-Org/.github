# Contributing to O-Tech Repos

Thanks for contributing. O-Tech projects aim to be practical, reproducible, and maker-friendly.

## Ways to contribute
- Report bugs (with reproduction steps + environment details)
- Improve docs (clarity is a superpower)
- Add features (small and focused is best)
- Add tests or simulation/mocks (especially for GPIO/audio/camera)

## Ground rules (lightweight, but real)
- Keep changes focused: one PR = one logical change
- Prefer readable code over clever code
- Avoid breaking backwards compatibility unless discussed
- No secrets or credentials in commits, issues, or logs

## Development setup (Python projects)
1. Create a venv
   - Windows (PowerShell):
     - `py -3.11 -m venv .venv`
     - `.venv\Scripts\activate`
   - Linux/macOS:
     - `python3 -m venv .venv`
     - `source .venv/bin/activate`

2. Install deps
   - `pip install -r requirements.txt` (if present)
   - `pip install -r requirements-dev.txt` (if present)
   - `pip install ruff pytest`

3. Run checks
   - Lint: `ruff check .`
   - Tests: `pytest -q`

## Commit & PR guidance
- Write clear commit messages (what + why)
- Include test notes in the PR description
- If it touches hardware behavior, document:
  - expected pins/peripherals
  - safe defaults
  - simulation/mocking strategy

## Code style
- Prefer small, composable functions
- Avoid magic numbers (make constants)
- Log failures with actionable messages
- Keep UIs stable: do not auto-close windows on errors

## Licensing
By contributing, you agree that your contributions are licensed under the repository’s license.
