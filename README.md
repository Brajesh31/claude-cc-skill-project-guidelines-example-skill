# claude-cc-skill-project-guidelines-example-skill

A Claude Code skill template for documenting project-specific engineering guidelines, architecture, code patterns, testing requirements, and deployment workflows.

## Overview

This repository demonstrates how to organize project knowledge into a focused skill for a specific software application. A project skill gives an AI coding assistant the context needed to work consistently within a codebase instead of relying on generic development assumptions.

The included example describes a full-stack application architecture. Treat its technology choices and conventions as an example, then adapt the instructions to the actual project where the skill will be used.

## What a Project Skill Should Contain

- A short project overview and product purpose.
- Architecture and major system boundaries.
- Technology stack and runtime versions.
- Repository and directory structure.
- Coding conventions and reusable patterns.
- API and data model conventions.
- Testing requirements.
- Security and configuration rules.
- Build, deployment, and release workflows.
- Known constraints and important non-goals.

## Example Technology Areas

The example skill covers a full-stack application with areas such as:

- Frontend application architecture.
- Backend service organization.
- Database and persistence.
- AI integration and structured outputs.
- Deployment infrastructure.
- End-to-end and unit testing.

These are illustrative areas, not mandatory technologies. Replace them with the actual tools and services used by the target project.

## Installation

Clone the repository into your Claude Code skills directory:

```bash
git clone https://github.com/Brajesh31/claude-cc-skill-project-guidelines-example-skill.git ~/.claude/skills/cc-skill-project-guidelines-example
```

For another Claude-compatible environment, use its supported skills directory and preserve the repository structure.

## Usage

Invoke the skill when working on a project that has its own architecture and engineering conventions:

```text
/cc-skill-project-guidelines-example
```

Before using the example in a real project, replace the illustrative project details with verified information from that codebase.

## How to Adapt the Template

### 1. Document the Architecture

Describe the major components, their responsibilities, communication paths, and data ownership. Include only details that are current and useful for implementation.

### 2. Record the Technology Stack

List languages, frameworks, databases, infrastructure, and key package versions. Distinguish required dependencies from optional tools.

### 3. Explain the Repository Structure

Identify important directories and explain where new code should be placed. Avoid documenting every file unless that detail changes development decisions.

### 4. Define Code Patterns

Include examples for common tasks such as creating an API endpoint, adding a UI feature, validating input, accessing data, and handling errors.

### 5. Define Testing Expectations

Document the test frameworks, commands, required coverage areas, and any environment setup needed to run tests.

### 6. Document Deployment

Explain build commands, environment configuration, release steps, health checks, and rollback procedures.

### 7. Keep the Instructions Current

Update the project skill when architecture, package versions, deployment, or engineering conventions change.

## Suggested Project Skill Structure

```text
project-skill/
├── SKILL.md
├── references/
│   ├── architecture.md
│   ├── code-conventions.md
│   ├── api-patterns.md
│   ├── database.md
│   ├── testing.md
│   └── deployment.md
└── README.md
```

A single `SKILL.md` may be sufficient for a small project. Split details into references when the root instructions become difficult to navigate.

## Quality Checklist

- Project name and purpose are accurate.
- Technology versions match the repository.
- Architecture boundaries are current.
- Directory guidance reflects the actual structure.
- Code examples follow existing conventions.
- Test commands work in the target environment.
- Deployment instructions are verified.
- Secrets and private configuration are excluded.
- Project-specific constraints are explicit.
- Outdated or contradictory rules are removed.

## Repository Contents

- `SKILL.md`: Example project-specific guidelines and architecture instructions.
- `README.md`: Template overview and adaptation workflow.

## Important Note

This repository is an example, not a drop-in description for every project. Do not apply its architecture or technology stack blindly. Inspect the target codebase and replace illustrative details before relying on the skill for implementation work.

## Practical Principle

A good project skill reduces repeated explanations and prevents avoidable mistakes. Keep it accurate, concise, and specific to the codebase it describes.
