# Project Structure Template

Use this structure for a local financial calculator.

```text
project-name/
  package.json
  README.md
  index.html
  vite.config.ts
  tsconfig.json
  src/
    main.tsx
    App.tsx
    styles.css
    calculations/
      productA.ts
      productB.ts
      tax.ts
      fees.ts
      timeline.ts
      comparison.ts
    data/
      productAFees.json
      productBFees.json
      defaultAssumptions.json
      translations.zh.json
      translations.de.json
    components/
      LanguageSwitcher.tsx
      InputForm.tsx
      ResultsSummary.tsx
      ResultsTable.tsx
      AssumptionsPanel.tsx
      DisclaimerBox.tsx
    tests/
      productA.test.ts
      productB.test.ts
      comparison.test.ts
      regressionScenarios.test.ts
```

## Rules

- Calculations must be pure functions.
- Components must not contain hardcoded fee parameters.
- JSON data must include source metadata.
- UI language strings must live in translation JSON files.
- Tests must run before visual refinements.
- Public repositories must contain only demo parameters unless real data is public and properly licensed.
