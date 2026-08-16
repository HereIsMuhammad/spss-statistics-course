# Day 4: Understanding Levels of Measurement (Nominal, Ordinal, Scale)

## Recap

We briefly touched on this in Day 1. Today we cover it properly, because this single concept decides which statistical test you are allowed to run on a variable. Getting this wrong is one of the most common mistakes beginners make in SPSS.

## Why Levels of Measurement Matter

SPSS is not just storing numbers, it needs to know **what kind of information** a number represents. A "2" could mean:

- The number of children someone has (a real quantity)
- The code for "Female" in a gender variable (just a label)
- A ranking of "somewhat satisfied" on a survey scale (an order, but not a real quantity)

These three are completely different, and SPSS handles them differently once you set the correct Measure in Variable View.

## The Three Levels

### 1. Nominal

Categories with **no meaningful order**. The numbers are just labels/codes, you could swap them and it would not change the meaning.

**Examples:**
- Gender (1 = Male, 2 = Female)
- Marital Status (1 = Single, 2 = Married, 3 = Divorced)
- City (1 = Lahore, 2 = Karachi, 3 = Islamabad)

**Tests you can run:** Frequencies, Mode, Chi-Square

### 2. Ordinal

Categories **with a meaningful order**, but the distance between categories is not equal or measurable.

**Examples:**
- Education Level (1 = High School, 2 = Bachelors, 3 = Masters)
- Satisfaction Rating (1 = Very Dissatisfied, 2 = Dissatisfied, 3 = Neutral, 4 = Satisfied, 5 = Very Satisfied)
- Income Bracket (1 = Low, 2 = Medium, 3 = High)

Notice: we know Masters is "higher" than Bachelors, but we cannot say the "distance" between High School and Bachelors is the same as between Bachelors and Masters.

**Tests you can run:** Median, Mode, Spearman Correlation, Mann-Whitney, Kruskal-Wallis

### 3. Scale

Numeric variables where the **distance between values is real and equal**, and where math operations (addition, averages) actually make sense.

**Examples:**
- Age (the difference between 20 and 25 is the same as between 40 and 45)
- Income in Rupees
- Test Scores
- Height, Weight

**Tests you can run:** Mean, Standard Deviation, Pearson Correlation, T-Test, ANOVA, Regression

## Quick Comparison Table

| Level | Order Matters? | Equal Distance? | Example | Common Tests |
|---|---|---|---|---|
| Nominal | No | No | Gender, City | Frequencies, Chi-Square |
| Ordinal | Yes | No | Satisfaction Rating, Education | Median, Spearman |
| Scale | Yes | Yes | Age, Income, Test Score | Mean, T-Test, ANOVA, Regression |

## How to Set This in SPSS

1. Go to Variable View
2. Find the **Measure** column for your variable
3. Click the cell, a dropdown appears
4. Select Nominal, Ordinal, or Scale

SPSS sometimes guesses this automatically on import, but it often guesses wrong (for example, it may mark a coded satisfaction rating as Scale). Always review and correct this manually.

## Common Mistake

A big mistake is running a Mean on a Nominal variable. For example, if gender is coded 1 = Male, 2 = Female, calculating the "average gender" (like 1.6) is meaningless. The Measure setting does not stop you from doing this in SPSS, so you must understand the concept yourself, SPSS will not always warn you.

## Practice Task

Take the dataset you imported on Day 3 and classify every variable:

| Variable | Correct Measure | Why |
|---|---|---|
| `id` | Nominal | Just an identifier, not a real quantity |
| `age` | Scale | Real numeric distance between values |
| `gender` | Nominal | Categories with no order |
| `monthly_income` | Scale | Real numeric distance between values |

Update the Measure column in Variable View to match.

## Key Takeaway

Before running any statistical test, always ask: "What level of measurement is this variable?" This single check prevents most of the wrong-test mistakes beginners make in SPSS.
