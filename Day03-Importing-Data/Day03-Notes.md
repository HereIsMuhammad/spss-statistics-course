# Day 3: Importing Data from Excel/CSV into SPSS

## Recap

On Day 2 we learned how to manually create variables and enter data directly in SPSS. In real projects, data usually already exists in Excel or CSV format (from Google Forms, surveys, or client files), so today we learn how to bring that data into SPSS properly.

## Why Import Instead of Manual Entry?

- Survey tools like Google Forms, SurveyMonkey, and Microsoft Forms export directly to Excel/CSV
- Clients on Upwork will almost always send you an Excel or CSV file, not a `.sav` file
- Manually retyping hundreds of rows is slow and error prone
- Importing keeps the original data safe as a backup

## Importing an Excel File

1. Open SPSS
2. Go to `File` then `Open` then `Data`
3. In the "Files of type" dropdown, select `Excel (*.xlsx, *.xls, *.xlsm)`
4. Browse and select your Excel file, click Open
5. A dialog box appears:
   - Check **"Read variable names from the first row of data"** if your Excel has column headers, this makes SPSS use those headers as variable names
   - Choose the correct **Worksheet** if the file has multiple sheets
   - Set the **Range** if you only want specific cells
6. Click OK, your data now loads into Data View

## Importing a CSV File

1. Go to `File` then `Open` then `Data`
2. Select `Text (*.txt, *.csv, *.tab)` from Files of type
3. Select your CSV file, this opens the **Text Import Wizard**
4. Follow the wizard steps:
   - Step 1: Choose "Delimited" (most CSVs are comma separated)
   - Step 2: Confirm variable names are in the first row
   - Step 3: Confirm the first case of data starts from the correct row
   - Step 4: Select "Comma" as the delimiter
   - Step 5: Review each column and set variable names if needed
   - Step 6: Click Finish

## What to Check After Importing

Importing rarely gets everything perfect on the first try, always check:

| Issue | What to Do |
|---|---|
| Variable names look messy (e.g. `What_is_your_age`) | Rename them in Variable View to something short like `age` |
| Numeric columns imported as String | Change Type to Numeric in Variable View, may need to fix invalid text first |
| Missing values shown as blank or "N/A" | Set proper Missing Values in Variable View (covered on Day 10) |
| No Value Labels for coded categories | Add Value Labels manually if the Excel had text categories converted to numbers |
| Measure column says "Unknown" | Set correct Measurement level (Nominal, Ordinal, Scale) for each variable |

## Common Beginner Mistake

If a numeric column has even a single non-numeric entry (like someone typing "twenty" instead of "20", or a stray space), SPSS may import the entire column as String. Always scan your Excel file for typos before importing, or fix the Type manually after import.

## Practice Task

1. Create a small Excel file with columns: `id`, `age`, `gender`, `monthly_income` (10 rows of sample data)
2. Save it as `.xlsx`
3. Import it into SPSS following the steps above
4. Check Variable View, fix any variable names, types, or measurement levels that look wrong
5. Save the cleaned file as `dataset.sav`

## Key Takeaway

Importing saves time, but it is not "set and forget." Always review Variable View after import, this single habit prevents most errors in later statistical tests.

---

**Next:** Day 4, Understanding levels of measurement (Nominal, Ordinal, Scale).