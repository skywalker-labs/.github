# Contributing to Skywalker Labs

Thank you for your interest in contributing to **Skywalker Labs** and the **Skywalker Intelligence System** open-source ecosystem!

We value precision, architectural craftsmanship, and clean design patterns. To maintain our high quality benchmarks across all 15+ open-source packages and systems, please adhere to the following standards when contributing.

---

## 📐 Code Quality & Formatting Benchmarks

Every pull request must adhere to the ecosystem standards for its target language:

### PHP / Laravel Codebases
- **Standards:** Strict compliance with PHP-FIG standards:
  - **PSR-1** / **PSR-4** autoloading
  - **PSR-7** HTTP message interfaces
  - **PSR-12** extended coding style guide
- **Static Analysis:** Audited through **PHPStan (Level 8)** or **Psalm** with zero unhandled errors.
- **Testing:** Comprehensive test suites using **Pest** or **PHPUnit** covering positive, edge, and failure paths.

### Python Codebases
- **Standards:** **PEP 8** style guidelines, enforced with Flake8/Black/Ruff.
- **Typing:** Strict type hints verified via `mypy`.
- **Testing:** Verified through **PyTest**.

### JavaScript / TypeScript / Frontend
- **Standards:** Strict ESLint and Prettier configurations.
- **Typing:** TypeScript strict mode enabled (`"strict": true`).

---

## 🌿 Git Branching & Commit Conventions

### Commit Messages
We follow the **Conventional Commits** specification:
```text
<type>(<scope>): <short description>

[optional body]

[optional footer(s)]
```
- `feat:` A new feature or capability.
- `fix:` A bug fix.
- `docs:` Documentation updates.
- `refactor:` Code changes that neither fix a bug nor add a feature.
- `test:` Adding or updating tests.
- `chore:` Build scripts, dependency bumps, or tool configurations.

### Branch Naming
- `feature/<short-name>`
- `fix/<issue-number>-<short-description>`
- `refactor/<target-area>`

---

## 🚀 Pull Request Workflow

1. **Fork the Repository** and clone your fork locally.
2. **Create a Feature Branch** (`git checkout -b feature/awesome-feature`).
3. **Write Clean, Tested Code**: Add test coverage for all new or modified code.
4. **Run Local Checks**: Ensure static analysis, linters, and test suites pass locally.
5. **Push to Your Fork** and open a Pull Request against `main`.
6. **Complete the PR Template**: Clearly describe the motivation, changes, and verification steps.

---

## ⚖️ Semantic Versioning (SemVer)

All repositories and packages adhere strictly to **SemVer (MAJOR.MINOR.PATCH)**:
- **PATCH:** Backward-compatible bug fixes.
- **MINOR:** Backward-compatible new functionality.
- **MAJOR:** Breaking API changes (must include deprecation warnings and migration guides).

