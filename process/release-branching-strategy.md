## Summary

This document defines the branching strategy used for FAIR project releases. 

## Core Principles

1. **Main is always production-ready** - The `main` branch represents the latest stable release
2. **Releases develop in isolation** - Each release has its own development branch
3. **Quality gates before merge** - All testing and validation happens before merging to main
4. **Automation supports humans** - CI/CD handles repetitive tasks; release managers shepherd the process

## Release Branch Workflow

### Overview

```mermaid
flowchart LR
    A[Create release/X.Y.Z branch] --> B[Development & PRs]
    B --> C[Testing & Validation]
    C --> D[Merge to main]
    D --> E[Automated release & deployment]
    E --> F[Delete release branch]
    F --> G[Next release cycle]
    G --> A
```

### Workflow Steps

1. **Create Release Branch**
   - Branch from `main` using the naming convention `release/X.Y.Z`
   - Example: `release/1.2.0`

2. **Development Phase**
   - All feature work and bug fixes for the release go into the release branch
   - Updates within a release do **not** go directly into `main`
   - Contributors open PRs against the release branch

3. **Testing & Validation**
   - QA and testing occur on the release branch
   - All CI checks must pass before the release is considered ready
   - Release manager coordinates validation efforts

4. **Merge to Main**
   - Once validated, the release branch is merged into `main` via PR
   - This triggers automated release actions and deployments
   - A version tag is created (e.g., `v1.2.0`)

5. **Cleanup**
   - The release branch is deleted after successful merge
   - The cycle repeats for the next release

### Branch Lifecycle

```mermaid
gitGraph
    commit id: "v1.0.0"
    branch release/1.1.0
    checkout release/1.1.0
    commit id: "feature A"
    commit id: "feature B"
    commit id: "bug fix"
    checkout main
    merge release/1.1.0 id: "v1.1.0" tag: "v1.1.0"
    branch release/1.2.0
    checkout release/1.2.0
    commit id: "feature C"
    commit id: "feature D"
    checkout main
    merge release/1.2.0 id: "v1.2.0" tag: "v1.2.0"
```

## Branch Protection

### Main Branch

The `main` branch requires strict protection rules:

| Rule | Setting |
|------|---------|
| Require pull request reviews | 1-2 reviewers minimum |
| Require status checks to pass | All CI tests |
| Require code owner approval | Enabled |
| Prevent force pushes | Enabled |
| Prevent deletions | Enabled |
| Restrict direct pushes | Only via PR |

### Release Branches

Release branches (`release/*`) should have these protections:

| Rule | Setting |
|------|---------|
| Require status checks to pass | All CI tests |
| Require pull request reviews | Recommended |
| Prevent force pushes | Enabled |
| Allow deletion | After merge to main |


## CODEOWNERS

A `CODEOWNERS` file should be placed in `.github/CODEOWNERS` to ensure appropriate review coverage.

## Automation

### GitHub Actions Workflow Structure

TBD

### Recommended Repository Settings

Enable these settings to support the workflow:

- **Automatically delete head branches** - Cleans up release branches after merge
- **Require branches to be up to date** - Prevents merge conflicts in main
- **Require linear history** - Optional, keeps git history clean

## Quick Reference

### Branch Naming Convention

| Branch Type | Pattern | Example |
|-------------|---------|---------|
| Release | `release/X.Y.Z` | `release/1.2.0` |
| Feature | `feature/description` | `feature/add-export` |
| Bugfix | `fix/description` | `fix/login-error` |
| Documentation | `docs/description` | `docs/api-guide` |
