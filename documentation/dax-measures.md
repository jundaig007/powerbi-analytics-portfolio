# DAX Measures

This file documents representative DAX patterns used in the portfolio project.

## Total Revenue

```DAX
Total Revenue =
SUM(Sales[Revenue])
```

## Previous Period Revenue

```DAX
Previous Period Revenue =
CALCULATE(
    [Total Revenue],
    DATEADD('Date'[Date], -1, MONTH)
)
```

## Revenue Growth %

```DAX
Revenue Growth % =
DIVIDE(
    [Total Revenue] - [Previous Period Revenue],
    [Previous Period Revenue],
    0
)
```

## Notes

Replace these representative measures with the actual sanitized measures used in the final portfolio dashboard. Document the business definition of every KPI, not only the DAX syntax.
