# Prompt: Create A Local Financial Calculator

Use this prompt with Codex or ChatGPT after replacing bracketed placeholders.

```text
Create a local financial model calculator.

Goal:
Build a browser-based local app for comparing:
1. [Product/model A]
2. [Product/model B]
3. Optional: [Product/model C]

Technology:
- React
- TypeScript
- Vite
- no backend by default
- no database
- no login
- no analytics
- no external API calls
- no customer data upload

Architecture:
- All calculation logic must be pure functions in src/calculations/.
- All fees, tax assumptions, product assumptions, and source metadata must be in JSON files under src/data/.
- UI components must not hardcode fee or tax parameters.
- Language strings must live in translation JSON files.
- The app must support [languages].

Inputs:
- [input 1]
- [input 2]
- [input 3]
- [input 4]

Outputs:
- total contributions / premiums
- value before tax
- total costs
- taxes
- value after tax
- difference between models when comparison is fair
- warning when inputs are not comparable
- explanation of why results differ

Data source metadata:
Every data file must include:
- sourceName
- sourceDate
- sourceUrl
- needsVerification

Testing:
Create unit tests for:
- lump sum only
- monthly contribution only
- combined lump sum and monthly contribution
- fee deduction order
- tax base
- final result
- timeline consistency

Important:
If benchmark results cannot be reproduced, do not polish the UI. Generate a debug report explaining formula differences, fee order, tax assumptions, and likely causes.

Compliance disclaimer:
This is a non-binding model calculation and does not constitute investment advice, tax advice, insurance advice, or a product recommendation.
```
