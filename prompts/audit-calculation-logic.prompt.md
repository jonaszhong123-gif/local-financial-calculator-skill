# Prompt: Audit Calculation Logic

```text
Audit the calculation logic of this local financial calculator.

Do not change UI styling.

Focus on:
1. Whether each model supports lump sum, monthly contribution, and combined inputs.
2. Whether fees are deducted in a clear, documented order.
3. Whether taxes are calculated only on the intended tax base.
4. Whether product wrappers and direct investments use separate tax logic.
5. Whether every parameter comes from JSON or structured data, not UI components.
6. Whether sourceName, sourceDate, sourceUrl, and needsVerification are present.
7. Whether timeline values match final result calculations.
8. Whether early exit, surrender, or liquidation values are clearly labelled as model estimates unless official values are provided.
9. Whether bilingual labels use professional terminology.
10. Whether the app avoids recommendation language.

Produce a validation report with:
- every formula
- every parameter source
- every test scenario
- current result
- target result
- difference
- likely reason
- whether UI refinement can proceed

If calculation logic is wrong, fix calculation first and do not polish UI.
```
