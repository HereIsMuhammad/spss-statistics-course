# Day 1: Introduction to SPSS

## What is SPSS?

SPSS (Statistical Package for the Social Sciences) is software made by IBM for statistical analysis. It is widely used by researchers, students, and businesses to analyze survey data, run statistical tests, and generate reports without writing code.

It is popular in fields like psychology, social sciences, marketing, healthcare, and education because it lets you perform complex statistics through a point and click interface.

## Why Use SPSS?

- No programming required, everything is menu based
- Handles large survey datasets easily
- Produces publication ready tables and charts
- Widely accepted in academic research (thesis and dissertations often require SPSS output)
- Has a syntax option too, so repeated analysis can be automated like code

## Installing SPSS

1. SPSS is a paid IBM product, but many universities provide free access through their library or IT department
2. A trial version is available on the IBM website for testing purposes
3. After installation, open the application, you will see a blank spreadsheet like interface

## Understanding the Interface

When you open SPSS, you will notice two main tabs at the bottom left of the window:

### 1. Data View

This is where your actual data lives. Each row represents one case (for example, one survey respondent), and each column represents one variable (for example, age, gender, income).

Think of it like an Excel sheet, but every column must follow rules defined in Variable View.

### 2. Variable View

This is where you define the properties of each variable before entering data. For every variable, you can set:

| Property | What it Means |
|---|---|
| Name | Short variable name (no spaces), e.g. `age`, `gender` |
| Type | Numeric, String, Date, etc. |
| Width | Number of characters/digits allowed |
| Decimals | Number of decimal places shown |
| Label | Full description of the variable, e.g. "Respondent Age in Years" |
| Values | Labels for coded numbers, e.g. 1 = Male, 2 = Female |
| Missing | Defines what counts as a missing value |
| Measure | Nominal, Ordinal, or Scale |

## Levels of Measurement (Preview)

You will study this in detail on Day 4, but it is useful to see it now:

- **Nominal**: categories with no order, e.g. gender, city
- **Ordinal**: categories with a meaningful order, e.g. education level (High School, Bachelors, Masters)
- **Scale**: numeric values with real distance between them, e.g. age, income

SPSS uses this classification to decide which statistical tests are appropriate later on.

## Other Important Windows

- **Output Viewer**: opens automatically when you run any analysis, this is where all your results (tables, charts) appear
- **Syntax Editor**: lets you write and save SPSS commands as code instead of clicking through menus, useful for repeating the same analysis on new data

## Practice Task

1. Open SPSS
2. Go to Variable View and create three variables: `id` (numeric), `name` (string), `age` (numeric)
3. Switch to Data View and enter 5 rows of sample data
4. Save the file as `.sav`

## Key Takeaway

SPSS separates **how your data is structured** (Variable View) from **the actual data** (Data View). Getting Variable View right from the start saves a lot of trouble later when running statistical tests.

---

**Next:** Day 2, Creating a dataset, variable names, types, labels, and value labels.