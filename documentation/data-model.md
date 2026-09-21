# Data Model

## Recommended Modeling Approach

Use a star-schema design where practical.

### Fact Tables
Contain measurable business events such as transactions, revenue, orders, usage, or operational activity.

### Dimension Tables
Common dimensions may include:

- Date
- Customer
- Product
- Location
- Business Unit
- Category

## Modeling Principles

- Prefer one-to-many relationships from dimensions to facts.
- Use a dedicated Date table for time intelligence.
- Avoid unnecessary bi-directional relationships.
- Keep business logic in reusable measures rather than repeated visual-level calculations.
- Standardize naming conventions and KPI definitions.
- Validate row counts and aggregate totals after transformation.
