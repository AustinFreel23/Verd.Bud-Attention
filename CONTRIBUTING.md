
# Contributing to Nomos

Thank you for your interest in contributing to **Nomos**, a reputation infrastructure for autonomous agents in the Web4 AI economy.

This document outlines the standards, workflows, and expectations for contributing to the Nomos repository. The goal is to maintain a high-quality, transparent, and collaborative development process.

---

# Table of Contents

1. Philosophy
2. Types of Contributions
3. Code of Conduct
4. Development Environment
5. Repository Structure
6. Contribution Workflow
7. Branching Strategy
8. Commit Guidelines
9. Pull Request Process
10. Documentation Contributions
11. Protocol Contributions
12. Issue Reporting
13. Security Issues
14. Review Process
15. Release Process
16. Community Standards

---

# Philosophy

Nomos is designed as open infrastructure for reputation-aware autonomous systems. Contributions should prioritize:

- clarity
- security
- reproducibility
- interoperability
- protocol neutrality

All contributions should help strengthen the ecosystem for trust-aware agent coordination.

---

# Types of Contributions

We welcome multiple types of contributions.

## Code Contributions

Examples include:

- protocol modules
- reputation computation models
- SDK implementations
- API services
- storage layers
- performance optimizations

## Documentation Contributions

Examples include:

- protocol documentation
- developer tutorials
- architecture diagrams
- API references
- integration examples

## Research Contributions

Examples include:

- trust modeling research
- behavioral signal modeling
- reputation scoring algorithms
- agent coordination models

## Tooling Contributions

Examples include:

- testing frameworks
- integration libraries
- monitoring tools
- data simulation tools

---

# Code of Conduct

All contributors are expected to maintain a professional and respectful environment.

Unacceptable behavior includes:

- harassment
- discrimination
- hostile communication
- intentional disruption of development processes

Contributors should focus on technical merit and collaborative progress.

---

# Development Environment

Nomos development assumes the following environment:

Recommended tools:

- Python 3.10+
- Node.js 18+
- Docker
- Git

Example setup:

```bash
git clone https://github.com/nomos/protocol.git
cd protocol
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

For local testing:

```bash
docker compose up
```

---

# Repository Structure

The repository follows a modular architecture.

```
nomos/
│
├── protocol/
│   ├── identity/
│   ├── trace/
│   ├── reputation/
│   └── attestations/
│
├── services/
│   ├── api/
│   ├── ingestion/
│   └── workers/
│
├── sdk/
│   ├── python/
│   └── typescript/
│
├── models/
├── storage/
├── scripts/
├── tests/
└── docs/
```

Contributors should place code in the appropriate module.

---

# Contribution Workflow

The recommended workflow is:

1. Fork the repository
2. Create a feature branch
3. Implement changes
4. Add tests where applicable
5. Submit a pull request

Example:

```bash
git fork https://github.com/nomos/protocol
git checkout -b feature/reputation-signal-model
```

---

# Branching Strategy

Nomos uses a structured branching model.

Main branches:

- `main` — stable production code
- `dev` — integration branch
- `feature/*` — feature development
- `fix/*` — bug fixes
- `research/*` — experimental research modules

Example:

```
feature/behavioral-signal-parser
feature/reputation-aggregation-engine
fix/event-validation-bug
```

---

# Commit Guidelines

Commit messages should be clear and structured.

Recommended format:

```
type(scope): description
```

Examples:

```
feat(identity): add agent identity validation
fix(trace): correct event timestamp validation
docs(protocol): update reputation model documentation
```

Allowed commit types:

- feat
- fix
- docs
- refactor
- test
- chore

---

# Pull Request Process

Pull requests should follow the following format.

Title example:

```
feat(reputation): introduce weighted signal model
```

Pull request description should include:

- summary of changes
- motivation
- testing strategy
- compatibility notes

Example template:

```
Summary:
Introduce weighted signal aggregation model.

Motivation:
Improve reputation stability for agents with diverse workloads.

Testing:
Unit tests added for signal weighting logic.
```

---

# Documentation Contributions

Documentation is critical for protocol adoption.

Documentation contributions may include:

- architecture diagrams
- developer guides
- protocol explanations
- integration tutorials

Documentation files should be placed in:

```
docs/
```

Preferred formats:

- Markdown
- ASCII diagrams
- structured examples

---

# Protocol Contributions

Changes affecting protocol behavior should include:

- detailed design description
- compatibility analysis
- migration considerations
- performance implications

Major protocol changes should include an RFC-style document.

Example structure:

```
docs/rfc/
```

---

# Issue Reporting

Issues should be reported with clear reproduction steps.

Example template:

```
Title: Trace ingestion fails on malformed event

Environment:
Python 3.11
Docker

Steps to reproduce:
1. Submit event with missing timestamp
2. Observe ingestion failure

Expected behavior:
Graceful rejection with error message
```

---

# Security Issues

Security issues should **not** be reported publicly.

Please report security concerns to:

```
security@nomosweb.org
```

Include:

- vulnerability description
- reproduction steps
- potential impact

Responsible disclosure is strongly encouraged.

---

# Review Process

All pull requests will be reviewed by maintainers.

Review criteria include:

- code quality
- architectural alignment
- protocol consistency
- security considerations
- documentation completeness

Maintainers may request changes before merging.

---

# Release Process

Nomos releases follow semantic versioning.

Format:

```
MAJOR.MINOR.PATCH
```

Example:

```
1.0.0
1.1.0
1.1.1
```

Release stages:

1. development
2. review
3. release candidate
4. stable release

---

# Testing Guidelines

All code contributions should include appropriate testing.

Recommended testing types:

- unit tests
- integration tests
- protocol simulation tests

Example test command:

```bash
pytest tests/
```

---

# Community Standards

Nomos aims to build an open ecosystem for autonomous agents.

Community members should:

- share research
- collaborate openly
- maintain technical integrity
- prioritize interoperability

Constructive feedback is encouraged.

---

# Getting Help

If you need help contributing, please open a discussion or issue in the repository.

Resources:

Website  
https://nomosweb.org/

Official Twitter  
https://x.com/nomosonx

---

# Final Note

Nomos is an open infrastructure project exploring the foundations of trust for autonomous systems.

Contributions from developers, researchers, and builders are welcome.
