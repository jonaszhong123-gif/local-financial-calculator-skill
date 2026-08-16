# Prompt: Simplify UI Without Reducing Function

```text
Simplify the current financial calculator UI.

Do not remove calculation features and do not change core formulas unless required to fix a bug.

Goal:
The user should understand within 5 seconds:
- what input is being modelled
- which models are being compared
- what the projected values are
- whether this is a fair comparison or a configuration simulation

UI structure:
1. Header
2. Product/model selection
3. Main inputs
4. Result cards
5. Short explanation
6. Optional chart
7. Collapsed professional details
8. Collapsed audit details
9. Disclaimer

Display modes:
1. Client view:
   - inputs
   - core result cards
   - short difference explanation
   - short disclaimer
2. Professional view:
   - chart
   - fees and taxes
   - model assumptions
3. Audit view:
   - formulas
   - detailed fee split
   - tax assumptions
   - source metadata
   - regression test references

Rules:
- Do not show long bilingual labels everywhere. Use the active language.
- Avoid negative differences when a human-readable phrase is clearer.
- Only show a higher model statement when inputs and assumptions are identical.
- If inputs differ, label as configuration simulation.
- Do not use recommendation language.
- Keep mobile width usable at 390px.
- Advanced sections should be collapsed by default.
```
