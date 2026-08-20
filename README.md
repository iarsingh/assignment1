# assignment1

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
