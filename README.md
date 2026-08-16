# Local Financial Calculator Skill Template

This repository is a public template for creating local, privacy-first financial model calculators with Codex or ChatGPT.

It is not a finished financial product and does not contain real client contracts, insurer documents, private fee tables, or verified tax advice.

## Purpose

Use this template to generate a local calculator such as:

- investment vs. insurance model comparison
- fund wrapper vs. direct brokerage account
- pension or withdrawal model projection
- client-facing advisory model with internal audit mode

The generated app should be:

- local-first
- testable
- transparent about formulas
- explicit about assumptions
- clear about legal and tax boundaries
- free of customer data upload

## Privacy Boundary

This template is safe to publish because it contains only:

- generic instructions
- sample data schemas
- prompt templates
- placeholder assumptions

Do not commit:

- real applications or contracts
- personal identifiers or private data
- local file paths
- internal review packages
- PDF screenshots
- scanned documents
- proprietary fee tables
- insurer-specific parameters unless they are publicly licensed and properly sourced

## Recommended Generated App Stack

- React
- TypeScript
- Vite
- pure calculation functions
- JSON assumption tables
- unit tests
- static web build

No backend is required for the default version.

## Static PWA Demo

A sanitized static demo can be published with GitHub Pages from the `docs/` folder:

https://jonaszhong123-gif.github.io/local-financial-calculator-skill/

The demo is a browser-only PWA build. It does not require a backend, database, analytics, external API, or customer data upload. Any product parameters in a public demo must be treated as non-binding model assumptions and replaced with locally verified, properly sourced values before professional use.

## Repository Structure

```text
SKILL.md
README.md
templates/
  project-structure.md
  data-schema.json
  disclaimer.zh-de.md
  validation-report.template.md
  test-scenarios.template.md
prompts/
  create-local-calculator.prompt.md
  audit-calculation-logic.prompt.md
  simplify-ui.prompt.md
  release-static-web.prompt.md
examples/
  demo-fees.sample.json
  demo-assumptions.sample.json
```

## How To Use

1. Copy the relevant prompt from `prompts/`.
2. Replace the placeholder product names, fee parameters, tax assumptions, and language requirements.
3. Provide only sanitized, non-private source summaries.
4. Ask Codex to generate the local app.
5. Run tests before UI refinement.
6. Keep all professional assumptions in JSON files with source metadata.

## Required Disclaimer

Any generated calculator must clearly state that it is a non-binding model calculation and not investment advice, tax advice, insurance advice, or a product recommendation.

## License

MIT. See `LICENSE`.
