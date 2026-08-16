# Publishing Checklist

Use this checklist before making the repository public on GitHub.

## Safe To Publish

This template repository may contain:

- generic prompts
- generic skill instructions
- generic project structure
- sample JSON schemas
- placeholder assumptions
- disclaimer templates
- testing templates

## Must Not Be Published

Do not publish:

- real client files
- application forms
- contracts
- policy documents
- PDFs
- screenshots
- internal review logs
- local file paths
- insurer-specific private fee tables
- personal identifiers
- email addresses
- financial account identifiers
- tax IDs
- contract identifiers

## Pre-Publish Checks

Run a repository-wide text scan for organization-specific private terms, local paths, document names, account identifiers, and internal review artifacts. Use your own approved secret-scanning tool if available.

Review any matches manually before publishing.

## Suggested GitHub Repository Settings

Recommended repository name:

```text
local-financial-calculator-skill
```

Recommended visibility:

```text
Public
```

Recommended description:

```text
Prompt and skill templates for creating local, privacy-first financial model calculators with React, TypeScript and Vite.
```

Recommended topics:

```text
codex
chatgpt
react
typescript
vite
financial-calculator
privacy-first
local-first
prompt-template
```

## Git Commands

From inside this folder:

```powershell
git init
git add .
git commit -m "Initial public skill template"
git branch -M main
git remote add origin https://github.com/<your-user>/local-financial-calculator-skill.git
git push -u origin main
```

If using GitHub CLI:

```powershell
gh repo create local-financial-calculator-skill --public --source . --remote origin --push
```
