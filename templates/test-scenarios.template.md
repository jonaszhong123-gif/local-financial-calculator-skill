# Test Scenarios Template

Replace the placeholder values with verified benchmark scenarios for your model.

## Scenario A: Lump Sum

Input:

```text
initialAmount = [amount]
monthlyAmount = 0
years = [years]
annualReturn = [percent]
```

Expected:

```text
productA_afterTax ~= [expected]
productB_afterTax ~= [expected]
tolerance = [amount or percent]
```

Explain tolerance:

```text
[rounding, monthly timing, day-count convention, source document rounding]
```

## Scenario B: Monthly Contribution

Input:

```text
initialAmount = 0
monthlyAmount = [amount]
years = [years]
annualReturn = [percent]
```

Expected:

```text
productA_afterTax ~= [expected]
productB_afterTax ~= [expected]
```

## Scenario C: Combined Input

Input:

```text
initialAmount = [amount]
monthlyAmount = [amount]
years = [years]
annualReturn = [percent]
```

Expected:

```text
combined_afterTax ~= [expected]
```

## Required Formula Tests

- annual rate to monthly equivalent
- lump sum compounding
- monthly contribution timing
- combined compounding
- fee deduction order
- tax base
- timeline final value equals final result
- zero input behavior
- negative gain tax behavior
