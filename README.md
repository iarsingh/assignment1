# assignment1

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
