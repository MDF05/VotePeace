# Contributing to VotePeace

We appreciate your interest in contributing! This document provides guidelines for contributing to the root monorepo.

## Getting Started

1.  **Choose a Sub-Project**: Decide if you want to contribute to the `VotePeace-Backend` or `VotePeace-Frontend`.
2.  **Read Specific Guides**:
    -   [Backend Contribution Guide](./VotePeace-Backend/CONTRIBUTING.md)
    -   [Frontend Contribution Guide](./VotePeace-Frontend/CONTRIBUTING.md)

## Monorepo Workflow

### Cloning
Clone the full repository:
```bash
git clone https://github.com/MDF05/VotePeace.git
```

### Branching Strategy
-   `main`: The stable production branch.
-   `develop`: The active development branch (if used).
-   `feat/feature-name`: Feature branches.
-   `fix/bug-name`: Bug fix branches.

### Committing
We use **Conventional Commits**:
-   `feat:` A new feature
-   `fix:` A bug fix
-   `docs:` Documentation only changes
-   `chore:` Build process or auxiliary tool changes

Example:
```bash
git commit -m "feat(backend): add email notification service"
```

## Pull Requests

1.  Ensure your code passes all tests in the respective sub-project.
2.  Update documentation if you change logic.
3.  Link the PR to an Issue if applicable.
