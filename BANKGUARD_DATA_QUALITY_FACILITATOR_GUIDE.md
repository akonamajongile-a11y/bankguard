# BankGuard Data Quality Facilitator Guide

The raw banking data is deliberately messy.

Learners should discover the problems themselves through
profiling, validation, joins and business-rule checks.

## Hidden data-quality issues

### Missing data
- income
- employment status
- city
- merchant IDs
- transaction amounts
- channels
- account fields

### Duplicates
- customer records
- branch records
- transaction IDs
- fraud-label transaction IDs

### Text problems
- upper/lower case
- leading/trailing spaces
- repeated spaces
- inconsistent categories
- inconsistent currencies

### Numeric problems
- negative transaction amounts
- zero amounts
- extremely large amounts
- currency-formatted numbers
- invalid ages

### Date problems
- mixed date formats
- invalid dates
- future transaction dates
- impossible dates

### Referential-integrity problems
- invalid customer IDs
- invalid account IDs
- invalid merchant IDs

### Banking business-rule problems
- negative or zero transaction amounts
- unusually large transactions
- future transactions
- impossible customer ages
- suspicious merchant risk categories

## Expected learner evidence

Learners should produce:

1. Data profiling notebook.
2. Data-quality report.
3. Cleaning decisions.
4. Cleaned CSV datasets.
5. Validation checks.
6. Integrated banking dataset.
7. Pandas analysis.
8. SQL analysis.
9. Visualisations.
10. Business recommendations.

Do not provide this guide to learners at the start of the project.
