# ABS Recorded Crime – Victims: FDV Victims by Sex, 2014–2024

## Project

This project uses published Australian Bureau of Statistics (ABS) data on victims of family and domestic violence-related offences by sex from 2014 to 2024.

The purpose of this project was to practise spreadsheet data cleaning, data documentation, use of Excel functions, and preparation of public-health-related data for descriptive analysis.

## Source

Australian Bureau of Statistics (ABS), *Recorded Crime – Victims*.

The dataset is based on published, aggregated ABS statistics. It does not contain confidential, individual-level, or identifiable data.

## Cleaning completed

- Restructured the source table into a long-format dataset.
- Standardised variable names and location labels.
- Preserved original ABS values in the `value` column.
- Converted numeric values into a separate `numeric_value` column.
- Retained `n.a.` and `n.p.` values as non-numeric entries rather than replacing them with zero.
- Added state and territory codes using `XLOOKUP` and a location reference table.
- Added `data_status` classifications using an `IF` formula.
- Added value categories for descriptive data checking.
- Retained the original ABS workbook as a reference file and created a separate cleaned working file.

## Files

- `raw_abs_rcv_fdv_2014_2024.xlsx`: Original ABS table downloaded for this project and retained as a reference file.
- `cleaned_abs_rcv_fdv_by_sex_2014_2024.xlsx`: Cleaned and documented working dataset.
- `data_dictionary.csv`: Variable descriptions, formats and cleaning notes.

## Important limitations

- `n.a.` means that data are not available or the calculation is not applicable.
- `n.p.` means that data are not published.
- These values were not converted to zero.
- Some locations and years may not be comparable because availability and publication rules differ.
- ABS notes and methodological information should be considered before interpreting trends or comparing locations.

## Tools used

- Google Sheets
- Excel `IF` formula
- Excel `XLOOKUP` function
- GitHub

## Skills demonstrated

- Spreadsheet data cleaning
- Data restructuring and documentation
- Handling non-numeric and unavailable values
- Creating lookup tables and standardised location codes
- Basic data-quality checks
- Ethical use and attribution of public data
