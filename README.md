# Healthcare Analytics Dashboard (Power BI)

A portfolio project that turns a deliberately messy 10-sheet hospital workbook into a clean data model and four dashboards.

## Dashboards

![Patient Demographics and Risk](dashboard1.png)

![Hospital Operations and Admissions](dashboard2.png)

![Disease and Public Health Surveillance](dashboard3.png)

![Financial and Quality Performance](dashboard4.png)

## The problem
The source data had duplicates, mixed date formats, placeholders like N/A, numbers stored as text, broken IDs and impossible values. Nothing could be trusted until it was cleaned.

## What I did
- **Cleaned** 10 tables in Power Query: removed exact duplicates (60 in Encounters, 40 in Billing), standardised text, fixed dates and numbers, set impossible values to null, and repaired broken keys from a trusted second source.
- **Modelled** the data as a star schema with Encounters at the centre, 10 relationships and a Calendar table.
- **Built** about 40 DAX measures and 4 dashboards: Patient Demographics & Risk, Hospital Operations & Admissions, Disease & Public Health Surveillance, and Financial & Quality Performance.

## Key findings
1. About 58% of the 37.9M billed is still unpaid.
2. About 19% of claims are denied.
3. North has about 9,973 cases per 100,000 people, nearly double East (about 5,131).
4. Hypertension, Type 2 diabetes and asthma lead the diagnoses.
5. About 24% of visits are High or Critical severity.

## Files
- `healthcare dataset.pbix`: the Power BI file
- `Healthcare_Dashboard.pdf`: all four dashboards

## Tools
Excel, Power Query, Power BI Desktop, DAX

*The dataset is synthetic. It contains no real patients.*
