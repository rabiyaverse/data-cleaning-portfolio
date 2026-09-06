# ABS Recorded Crime – Victims: FDV by Sex, 2014–2024

## Project overview

This project uses published Australian Bureau of Statistics (ABS) data on victims of family and domestic violence-related offences by sex from 2014 to 2024.

The purpose of this project was to practise spreadsheet data cleaning, data documentation, spreadsheet functions, and preparation of public-health-related data for descriptive analysis.

## Source and attribution

Based on Australian Bureau of Statistics data.

Source dataset: Australian Bureau of Statistics (ABS), *Recorded Crime – Victims*.

The dataset is based on published, aggregated ABS statistics. It does not contain confidential, individual-level, or identifiable data.

## Cleaning and documentation completed

- Restructured the source table into a long-format dataset.
- Standardised variable names and location labels.
- Preserved original ABS values in the `value` column.
- Converted available text values with commas, such as `19,918`, into a separate `numeric_value` column for analysis.
- Retained `n.a.` and `n.p.` values as non-numeric entries rather than replacing them with zero.
- Added state and territory codes using `XLOOKUP` and a location reference table.
- Added `data_status` classifications using an `IF` formula.
- Used `COUNTIF` in the data-profile worksheet to count blank numeric values and identify records containing ABS special values such as `n.a.` and `n.p.`.
- Added value categories for descriptive data checking.
- Retained the original ABS workbook as a reference file and created a separate cleaned working file.

## Project workbook

`abs_fdv_data_cleaning_portfolio.xlsx` is the final workbook for this project.

It includes:

- `Cleaned_Data`: Structured long-format data prepared for descriptive analysis.
- `Data_Profile`: Data summary and data-quality checks.
- `Lookup_Reference`: Location-to-state and territory codes used with `XLOOKUP`, if included in the workbook.
- `Methods`: Cleaning steps, source information, formulas and limitations, if included in the workbook.

The workbook was checked before upload and contains no visible `#REF!`, `#VALUE!`, or `#N/A` formula errors.

## Important limitations

- `n.a.` means data are not available or the calculation is not applicable.
- `n.p.` means data are not published.
- These values were not converted to zero.
- Some locations and years may not be comparable because availability and publication rules differ.
- ABS notes and methodological information should be considered before interpreting trends or comparing locations.
- Recorded crime data describe incidents recorded by police and should not be interpreted as the total prevalence of family and domestic violence.

## Tools and functions used

- Google Sheets
- Excel `IF` formula
- Excel `COUNTIF` function
- Excel `XLOOKUP` function
- GitHub

## Skills demonstrated

- Spreadsheet data cleaning
- Data restructuring and documentation
- Data profiling and quality checks
- Handling non-numeric, unavailable and unpublished values
- Creating lookup tables and standardised location codes
- Applying spreadsheet formulas for classification, lookup and conditional counting
- Ethical use and attribution of public data
