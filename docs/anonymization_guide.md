# Anonymization Guide

Use this before publishing a portfolio repo or public case study.

## Remove Or Replace

- company names
- company logos
- customer names
- vendor or distributor names
- email addresses
- order IDs
- purchase order numbers
- employee names
- internal file names
- API keys
- credentials
- real business volumes
- confidential product names

## Use Synthetic Replacements

| Real Item | Public Replacement |
| --- | --- |
| Company name | ExampleCo |
| Customer name | CityCare Hospital |
| Distributor name | Northline Distributors |
| Email address | user@example.com |
| Product name | Product A 500mg |
| Order ID | ORD-2026-001 |
| Internal system | Downstream ERP |

## Screenshot Options

Best options:

1. Recreate the screen using dummy data.
2. Blur or cover sensitive parts.
3. Crop the screenshot to show only the interaction.
4. Use synthetic sample screenshots.

Avoid uploading raw screenshots if they contain live data.

## Video Options

For video snippets:

- cover logos with blur or a clean overlay
- avoid showing internal email IDs
- trim clips to the animation or interaction moment
- keep subtitles if they are generic
- do not include raw voiceover if it mentions confidential details

## Final Public Review

Before publishing, ask:

- Could someone identify the organization?
- Could someone identify a customer or vendor?
- Does any screen show real data?
- Does any filename reveal internal context?
- Are there hidden files with secrets?
- Does the commit history contain removed secrets?

If the answer to any question is yes, sanitize before upload.

