# Day 5: Frequencies and Frequency Tables

## Recap

On Day 4 we learned that a variable's level of measurement decides which tests we can run. Today we start actually running our first analysis: Frequencies, this works on Nominal, Ordinal, and even Scale variables, making it a great starting point for exploring any dataset.

## What is a Frequency Analysis?

A frequency analysis counts how many times each value appears in a variable. It answers the simple question: "How many respondents fall into each category?"

**Example:** If you have a `gender` variable, a frequency table tells you how many respondents are Male and how many are Female, along with percentages.

## Why Start Analysis with Frequencies?

- It is the fastest way to check your data was entered/imported correctly
- It reveals miscoded values immediately, for example if `gender` is supposed to only have 1 and 2 but a frequency table shows a stray 5, you know there is a data entry error
- It gives you a first overview before running deeper tests
- Clients and thesis readers often want a simple "how many responded what" table before anything else

## Running Frequencies in SPSS

1. Go to `Analyze` then `Descriptive Statistics` then `Frequencies`
2. Move the variable(s) you want to analyze into the "Variable(s)" box
3. Click `Statistics` if you also want Mean, Median, Mode shown here (optional, we cover this properly on Day 6)
4. Click `Charts` if you want a Bar Chart or Pie Chart of the results
5. Click OK

## Reading the Output

The Frequency table has four columns:

| Column | What it Means |
|---|---|
| Frequency | Raw count of how many cases have that value |
| Percent | Percentage out of ALL cases, including missing |
| Valid Percent | Percentage out of only the valid (non-missing) cases |
| Cumulative Percent | Running total percentage as you go down the categories |

**Important:** Always report **Valid Percent** in your results, not Percent, unless you specifically want to highlight how much data was missing.

## Example

If 100 people were surveyed on gender, but 5 left it blank:

| Gender | Frequency | Percent | Valid Percent |
|---|---|---|---|
| Male | 60 | 60.0% | 63.2% |
| Female | 35 | 35.0% | 36.8% |
| Missing | 5 | 5.0% | - |
| Total | 100 | 100.0% | 100.0% |

Notice Valid Percent is calculated out of 95 (the valid responses), not 100.

## When to Use Frequencies vs Descriptive Statistics

- Use **Frequencies** for Nominal and Ordinal variables (categories), since you want to see counts per category
- Use **Descriptives** (covered Day 6) for Scale variables like age or income, since counting every unique value is not useful, you want Mean/SD instead

Running Frequencies on a Scale variable like `age` with many unique values (18, 19, 20, 21...) will give you a long, messy, unhelpful table.

## Practice Task

Using your dataset from Day 3:

1. Run Frequencies on `gender` and `education`
2. Add a Bar Chart for each
3. Check if any unexpected values appear (like a code that should not exist)
4. Write down the Valid Percent for each category

## Key Takeaway

Frequencies is your first line of defense against bad data. Before running any advanced test, always run Frequencies on your categorical variables to catch errors early.
