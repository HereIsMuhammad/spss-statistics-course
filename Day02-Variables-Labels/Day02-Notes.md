# Day 2: Creating a Dataset, Variable Names, Types, Labels, and Value Labels

## Recap

On Day 1 we saw that Variable View defines the structure of your data, and Data View holds the actual values. Today we go deeper into how to properly set up variables before entering any data.

## Variable Names

Every variable needs a short, code friendly name. SPSS has rules for this:

- Must start with a letter (not a number or symbol)
- No spaces allowed, use underscores instead, e.g. `study_hours` not `study hours`
- Maximum length is 64 characters, but shorter is better
- Cannot use reserved words like `all`, `and`, `or`, `by`
- Case does not matter, `Age` and `age` are treated the same

Good practice: keep names short and meaningful, e.g. `gender`, `income`, `q1`, `q2` for questionnaire items.

## Variable Types

When you set up a variable in Variable View, you choose its Type:

| Type | Use Case |
|---|---|
| Numeric | Numbers, e.g. age, income, test scores |
| String | Text, e.g. name, city, open ended answers |
| Date | Dates, e.g. date of birth, survey date |
| Comma/Dot | Numbers displayed with thousand separators |

Most statistical analysis in SPSS needs Numeric or coded Numeric variables (not String), because SPSS calculates statistics only on numbers.

## Variable Labels vs Value Labels

This is one of the most confusing parts for beginners, so here is the difference clearly:

### Variable Label
This is the **full description** of the column itself.

Example: your variable name is `gender`, but its label could be `Respondent's Gender`. The label shows up in output tables instead of the short name, making results easier to read.

### Value Labels
This is used when your data is **coded with numbers** that represent categories.

Example: for the variable `gender`, you might enter:
- 1 = Male
- 2 = Female

So in Data View you only type `1` or `2`, but SPSS displays "Male" or "Female" in outputs if value labels are turned on. This keeps your dataset numeric (which SPSS prefers) while still being readable.

### Quick Comparison

| | Variable Label | Value Labels |
|---|---|---|
| What it describes | The column/variable | The individual codes inside a variable |
| Example | "Respondent's Gender" for `gender` | 1 = Male, 2 = Female |
| Where it is set | Variable View, Label column | Variable View, Values column |

## Why Coding Categories as Numbers Matters

Many beginners type "Male" and "Female" directly as text (String type). This works for basic viewing, but:

- You cannot run most statistical tests on String variables
- Numeric coding (1, 2, 3...) with Value Labels lets you keep data clean AND readable
- This is the standard approach used in real research and by data analysts

## Step by Step: Creating a Coded Variable

1. Go to Variable View
2. Type the variable name, e.g. `gender`
3. Set Type to Numeric
4. In the Label column, type `Respondent's Gender`
5. Click the Values cell, a small button (...) appears, click it
6. Add: Value = 1, Label = Male, click Add
7. Add: Value = 2, Label = Female, click Add
8. Click OK
9. Go to Data View and enter only `1` or `2` for each respondent

## Practice Task

Create a small dataset with these variables:

| Variable Name | Type | Label | Value Labels |
|---|---|---|---|
| `id` | Numeric | Respondent ID | none |
| `gender` | Numeric | Gender | 1 = Male, 2 = Female |
| `education` | Numeric | Education Level | 1 = High School, 2 = Bachelors, 3 = Masters |
| `income` | Numeric | Monthly Income | none |

Enter 8 to 10 rows of sample data, save it as `dataset.sav`.

## Key Takeaway

Always code categorical data as numbers and use Value Labels to make it readable. This single habit makes almost every later analysis (frequencies, cross tabs, t-tests) work correctly in SPSS.
