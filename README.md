# assignment1

## Overview

A Jenkins practice repository for running a declarative pipeline against a `develop`-based Git workflow. The root `Jenkinsfile` has a Checkout stage that pulls the `develop` branch, with the remaining stages left as placeholders. A copy of the same pipeline sits in `Assignment1/` with an empty test file to try running it from a subdirectory, and a `feature-branch` exists for practicing branch-based triggers.

- **Built with:** Jenkins declarative pipeline, Git
- **Scope:** Course assignment sandbox; the build and test stages are placeholders and nothing is deployed.

<!-- project-guide:start -->
## Project guide

[Project architecture](PROJECT_ARCHITECTURE.md) · [Interview questions and answers](INTERVIEW_QA.md)

Use the architecture document for the component diagram, implementation boundaries, and verification entry points. The interview guide includes source-backed answers and project walkthroughs.

### Implementation map

| Component | Responsibility |
| --- | --- |
| [`README.md`](README.md) | Project explanations or operating notes |

Setup and examples are described in the existing project notes below. Consult the component-specific manifests before assuming a single launch command.

<!-- project-guide:end -->

<!-- repository-summary -->
A Jenkins declarative-pipeline exercise using a develop-based Git workflow and placeholder build and test stages.
<!-- /repository-summary -->

A small Jenkins CI/CD practice repository for testing a declarative pipeline
against a `develop`-based Git workflow.

## What's here

- **`Jenkinsfile`** (root) — a declarative Jenkins pipeline with a
  `Checkout` stage that pulls the `develop` branch of this repo
  (`https://github.com/akhileshranjan2308/assignment1`). Remaining stages
  are left as placeholders (`// ... (other stages)`).
- **`Assignment1/`** — contains a copy of the same `Jenkinsfile` plus an
  empty `test.txt`, used to try out the pipeline running from a
  subdirectory instead of the repo root.

## Branches

The remote includes `develop` (default) and `feature-branch`, reflecting
that this repo is primarily a sandbox for practicing branch-based Jenkins
pipeline triggers rather than a deployable application.

## Usage

Point a Jenkins job at this repository (branch `develop`) to pick up the
pipeline defined in the root `Jenkinsfile`.

## Documentation checks

Project architecture, interview guides, and local source links are checked automatically on pushes and pull requests. Run the same check locally:

```bash
python3 .github/scripts/validate_project_docs.py
```
