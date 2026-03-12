# CLAUDE.md

This file provides guidance for AI assistants (Claude and others) working in this repository.

## Repository Overview

**MY-PT** is a project repository by hsolemio-lee. This file will be updated as the project structure and conventions are established.

> **Note:** This repository is currently in its initial state. Update this file as the project grows to reflect the actual stack, workflows, and conventions.

## Project Status

- [ ] Technology stack chosen
- [ ] Project structure initialized
- [ ] Development environment documented
- [ ] Testing strategy defined
- [ ] CI/CD configured

---

## Getting Started

### Prerequisites

_Document required tools and versions here (e.g., Node.js 20+, Python 3.11+, Docker, etc.)_

### Installation

```bash
# Clone the repository
git clone <repo-url>
cd MY-PT

# Install dependencies (update with actual commands)
# npm install
# pip install -r requirements.txt
# etc.
```

### Environment Setup

_Document required environment variables here. Example:_

```bash
# Copy the example env file and fill in values
cp .env.example .env
```

Key environment variables:
| Variable | Description | Required |
|----------|-------------|----------|
| _TBD_ | _TBD_ | _TBD_ |

---

## Project Structure

_Update this section once the project structure is established._

```
MY-PT/
├── CLAUDE.md          # This file
├── README.md          # Project documentation (add when ready)
└── .git/              # Git metadata
```

---

## Development Workflow

### Branch Naming

- Feature branches: `feature/<short-description>`
- Bug fixes: `fix/<short-description>`
- AI-assisted branches: `claude/<task-id>`
- Hotfixes: `hotfix/<short-description>`

### Commit Messages

Use clear, descriptive commit messages following this format:

```
<type>: <short summary>

<optional body explaining why, not what>
```

Types: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `style`

Examples:
- `feat: add user authentication`
- `fix: resolve null pointer in payment processor`
- `docs: update API endpoint documentation`

### Making Changes

1. Create a feature branch from the default branch
2. Make focused, atomic commits
3. Write or update tests for your changes
4. Ensure all tests pass before pushing
5. Open a pull request with a clear description

---

## Testing

_Update this section once a testing framework is chosen._

```bash
# Run all tests
# npm test / pytest / go test ./... / etc.

# Run tests in watch mode
# npm run test:watch

# Run with coverage
# npm run test:coverage
```

**Testing conventions:**
- Write tests alongside source code
- Aim for meaningful coverage on business logic
- Keep tests fast and deterministic

---

## Code Quality

_Update with actual linter/formatter commands once configured._

```bash
# Lint
# npm run lint / flake8 / golangci-lint run

# Format
# npm run format / black . / gofmt ./...

# Type check
# npm run typecheck / mypy . / tsc --noEmit
```

---

## Key Conventions

_Document project-specific conventions here as they are established. Examples:_

- **Naming:** Use camelCase for variables/functions, PascalCase for classes/components
- **File organization:** Group by feature, not by type
- **Error handling:** Always handle errors explicitly; avoid silent failures
- **Comments:** Write comments for "why", not "what"
- **Dependencies:** Prefer well-maintained, minimal dependencies

---

## Common Tasks

_Fill in with actual commands as the project grows._

| Task | Command |
|------|---------|
| Start dev server | _TBD_ |
| Run tests | _TBD_ |
| Build for production | _TBD_ |
| Deploy | _TBD_ |
| Database migrations | _TBD_ |

---

## Architecture & Design Decisions

_Document significant architectural decisions here as they are made. Include context and reasoning._

### ADR Template

When making a significant decision, document it:

```
## Decision: <title>
**Date:** YYYY-MM-DD
**Status:** Accepted / Deprecated / Superseded

### Context
Why was this decision needed?

### Decision
What was decided?

### Consequences
What are the trade-offs?
```

---

## Working with AI Assistants

### Guidance for Claude

- **Read before editing:** Always read files before modifying them
- **Minimal changes:** Make only the changes necessary for the task
- **No unnecessary files:** Do not create files unless required
- **Security:** Never introduce SQL injection, XSS, command injection, or other OWASP vulnerabilities
- **Test changes:** Run tests after making changes when possible
- **Commit messages:** Use the format described in the Development Workflow section
- **Branch:** Work on the specified `claude/` branch; never push to main/master without explicit permission

### Prohibited Actions (without explicit user approval)

- Force pushing to any branch
- Deleting branches or files containing important work
- Running destructive database operations
- Pushing to main/master
- Modifying CI/CD pipelines that affect production

---

## Resources

_Add links to relevant documentation, design docs, runbooks, etc. as the project grows._

- Repository: [hsolemio-lee/MY-PT](https://github.com/hsolemio-lee/MY-PT)
- Issues: [GitHub Issues](https://github.com/hsolemio-lee/MY-PT/issues)
