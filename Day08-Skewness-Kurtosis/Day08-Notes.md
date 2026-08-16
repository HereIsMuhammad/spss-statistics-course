# Day 8: Skewness & Kurtosis

## Recap

On Day 7 we learned how spread out data is (Range, Variance, SD). Today we learn about the **shape** of the data distribution, specifically whether it leans to one side (Skewness) and how "peaked" or "flat" it is (Kurtosis). This connects directly to Day 14, where we test for Normality.

## Why Shape Matters

Many statistical tests (T-Test, ANOVA, Regression, Pearson Correlation) assume your data follows a roughly **normal distribution** (the classic bell curve). If your data is heavily skewed or has an unusual shape, using these tests can give misleading results, and you may need a non-parametric test instead.

## What is a Normal Distribution?

A normal distribution is symmetric, shaped like a bell curve, where most values cluster around the Mean and taper off equally on both sides. Mean, Median, and Mode are all roughly equal in a perfectly normal distribution.

## 1. Skewness

Skewness measures whether your data leans more to one side than the other.

### Positive Skew (Right Skew)
- A long tail stretches toward the higher values
- Most data is clustered on the lower end, with a few very high values pulling the tail right
- **Example:** Income data, most people earn moderate amounts, but a few very high earners stretch the tail to the right
- Mean > Median in this case

### Negative Skew (Left Skew)
- A long tail stretches toward the lower values
- Most data is clustered on the higher end, with a few very low values pulling the tail left
- **Example:** Age at retirement, most people retire around a similar age, but a few retire very early, pulling the tail left
- Mean < Median in this case

### No Skew (Symmetric)
- Data is evenly balanced on both sides of the Mean
- Mean ≈ Median

## Interpreting the Skewness Value in SPSS

SPSS gives you a Skewness statistic along with its Standard Error.

| Skewness Value | Interpretation |
|---|---|
| Close to 0 | Roughly symmetric (normal-like) |
| Greater than +1 | Strong positive (right) skew |
| Less than −1 | Strong negative (left) skew |
| Between −1 and +1 | Acceptable for most analyses |

A common rule of thumb: divide Skewness by its Standard Error, if the result is beyond ±1.96 (roughly), the skew is statistically significant.

## 2. Kurtosis

Kurtosis measures how "peaked" or "flat" your distribution is compared to a normal distribution, essentially describing how much data sits in the tails versus the center.

### Types of Kurtosis

- **Mesokurtic (Kurtosis ≈ 0):** Normal peak, matches a standard bell curve
- **Leptokurtic (Kurtosis > 0):** Sharper, taller peak, more data clustered near the Mean, with heavier tails (more extreme outliers than normal)
- **Platykurtic (Kurtosis < 0):** Flatter peak, data more evenly spread out, fewer extreme outliers

## Quick Comparison Table

| Measure | What it Describes | Positive Value Means | Negative Value Means |
|---|---|---|---|
| Skewness | Symmetry (left/right lean) | Long tail to the right | Long tail to the left |
| Kurtosis | Peakedness | Sharper peak, heavier tails | Flatter peak, lighter tails |

## Running This in SPSS

1. `Analyze` then `Descriptive Statistics` then `Descriptives`
2. Move your Scale variable(s) into the box
3. Click `Options`
4. Check: Skewness and Kurtosis
5. Click Continue, then OK

You can also see this visually by requesting a Histogram with a normal curve overlay (`Analyze` then `Descriptive Statistics` then `Frequencies` then `Charts` then `Histogram` then check "Show normal curve").

## Practice Task

Using your dataset from Day 3:

1. Run Skewness and Kurtosis for `monthly_income` and `age`
2. Check if the Skewness value is beyond +1 or −1 for either variable
3. Generate a Histogram with a normal curve for `monthly_income` to visually confirm the skew
4. Write one sentence, for example: "Monthly income showed a skewness of 1.8, indicating a strong positive skew, likely due to a small number of high income respondents."

## Key Takeaway

Skewness and Kurtosis tell you whether your data behaves like a normal bell curve. This directly determines whether you can safely run parametric tests (T-Test, ANOVA, Pearson) or whether you need non-parametric alternatives, a decision we finalize with formal Normality Testing on Day 14.
