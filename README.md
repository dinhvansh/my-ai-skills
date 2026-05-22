# My AI Skills

A personal skill library for AI-assisted software engineering, business analysis, documentation, security review, automation, and project handover workflows.

This repository is designed to store reusable `SKILL.md` files that can be used with tools such as Claude Code, Codex-style agents, or any AI coding assistant that supports project-specific instructions.

## Repository Structure

```txt
my-ai-skills/
  README.md
  skills/
    project-documentation-cleanup/
      SKILL.md
  templates/
    documentation-audit-report.md
  examples/
    e-office/
      README.md
```

## Available Skills

| Skill | Purpose | Best For |
|---|---|---|
| `project-documentation-cleanup` | Clean up and rewrite project Markdown documentation after development | Project handover, maintenance, AI onboarding |

## How To Use

Copy the required skill folder into your target project.

Example for Claude Code:

```txt
.claude/skills/project-documentation-cleanup/SKILL.md
```

Example for a generic agent workspace:

```txt
.skills/project-documentation-cleanup/SKILL.md
```

Then ask the AI assistant to use the skill before working on the task.

Example prompt:

```md
Use the project-documentation-cleanup skill.
Scan the current repository, classify all Markdown files, create a documentation audit report, then rewrite the final documentation set based on the current codebase.
```

## Skill Design Principles

- Source code is the source of truth.
- Old Markdown files are references, not final truth.
- Do not delete old documents permanently.
- Archive draft, outdated, duplicate, or unclear documents.
- Do not invent features that are not implemented.
- Mark unclear areas as `TODO: Verify with source owner`.
- Do not expose secrets from `.env`, config files, logs, or old documents.

## Planned Skills

Potential future skills:

| Skill | Purpose |
|---|---|
| `project-security-review` | Review authentication, authorization, file access, secrets, and audit risks |
| `business-analysis-docs` | Generate BA documents such as BRD, user stories, workflow, permission matrix |
| `codebase-refactor-review` | Review architecture, code structure, duplication, and refactor priorities |
| `power-platform-review` | Review Power Apps, SharePoint, Power Automate, and governance rules |
| `n8n-automation-review` | Review n8n workflows, credentials, retries, error handling, and deployment |
| `qa-test-plan-generator` | Generate test plans, test cases, and regression checklists |

## Recommended Workflow

```txt
AI drafts or updates documentation
↓
Tech Lead verifies against source code
↓
BA verifies business workflow
↓
QA creates test checklist
↓
PM / Owner approves final version
```

## Notes

This repository is a living library. Add new skills as reusable folders under `skills/` and keep shared templates under `templates/`.
