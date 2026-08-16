# Local Financial Calculator Skill

Use this skill when a user wants to create, audit, or refine a local financial model calculator where privacy, explainability, and testability matter.

## Core Requirements

Generated calculators must:

- run locally by default
- avoid customer data upload
- avoid external APIs unless explicitly requested
- keep all calculation logic in pure functions
- keep all fees, assumptions, tax rates, and source metadata in JSON or structured data files
- support unit tests for every material formula
- clearly separate client-facing output from professional assumptions and audit details
- include legal, tax, and source-verification disclaimers

## Architecture Pattern

Use this default structure:

```text
src/
  calculations/
  data/
  components/
  tests/
```

Calculation modules should expose pure functions:

```ts
type CalculationInput = {
  initialAmount: number;
  monthlyAmount: number;
  years: number;
  annualReturnRate: number;
};

type CalculationResult = {
  totalContributed: number;
  valueBeforeTax: number;
  totalCosts: number;
  tax: number;
  valueAfterTax: number;
  timeline: TimelinePoint[];
};
```

## Data Source Rules

Every assumption file must include:

```json
{
  "sourceName": "Manual sample assumptions",
  "sourceDate": "YYYY-MM-DD",
  "sourceUrl": null,
  "needsVerification": true
}
```

Do not hardcode product fees inside UI components.

## Privacy Rules

Never include:

- personal identifiers
- scanned contracts
- application PDFs
- local user paths
- private email addresses
- financial account identifiers
- contract identifiers
- internal ChatGPT review logs
- unlicensed proprietary tables

If a user provides private material, summarize only the necessary sanitized assumptions and mark them as `needsVerification: true`.

## UI Pattern

Use three information levels:

1. Client view: inputs, core results, short disclaimer.
2. Professional view: charts, assumptions, cost and tax summary.
3. Audit view: formulas, source metadata, regression scenarios, detailed tables.

Do not use recommendation language such as:

- best product
- guaranteed return
- should buy
- safe profit

Prefer:

- model value
- projected value
- simplified estimate
- configuration simulation
- non-binding model calculation

## Testing Gate

Before UI polishing, run formula tests. If target scenarios cannot be reproduced, create a debug report instead of improving visuals.

Required tests should cover:

- lump sum only
- monthly contribution only
- combined lump sum and monthly contribution
- tax on gains only
- fee deduction order
- early exit or liquidation boundary if applicable
- timeline consistency

## Release Pattern

Default release should be a static web app:

- `npm run build`
- `dist/`
- no backend
- no database
- no login
- no analytics

If mobile access or real-time sync is required, state clearly that this requires a local service or hosted deployment and changes the privacy/security boundary.
