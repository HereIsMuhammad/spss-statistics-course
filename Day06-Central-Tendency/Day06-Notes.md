# Day 6: Measures of Central Tendency (Mean, Median, Mode)

## Recap

On Day 5 we used Frequencies to count categories. Today we move to Scale variables (like age, income, test scores) and learn how to summarize them with a single representative number using Mean, Median, and Mode.

## What is Central Tendency?

Central tendency answers the question: "What is the typical or central value in this data?" There are three ways to measure this, and each one behaves differently depending on your data.

## 1. Mean (Average)

The Mean is the sum of all values divided by the number of values.

**Formula:** Mean = (Sum of all values) / (Number of values)

**Example:** Ages: 20, 22, 23, 25, 60
Mean = (20+22+23+25+60) / 5 = 150 / 5 = 30

**When to use it:** Scale data that does not have extreme outliers.

**Problem:** The Mean is heavily affected by extreme values (outliers). In the example above, one person aged 60 pulled the average up to 30, even though most people in the group are in their early twenties. This is misleading.

## 2. Median

The Median is the middle value when all data is sorted from smallest to largest.

**Example:** Same ages sorted: 20, 22, 23, 25, 60
Median = 23 (the middle value)

**When to use it:** When your data has outliers or is skewed. The Median is not affected by extreme values, making it a more honest "typical value" in the example above (23 represents the group better than 30).

**Rule for even number of values:** Take the average of the two middle numbers.
Example: 20, 22, 23, 25 → Median = (22+23)/2 = 22.5

## 3. Mode

The Mode is the value that appears most frequently in the data.

**Example:** Ages: 20, 22, 22, 23, 25
Mode = 22 (appears twice, more than any other value)

**When to use it:** Useful for Nominal data (like the most common category), and also works for Scale data to spot the most repeated value. A dataset can have more than one Mode (bimodal, multimodal), or no Mode at all if every value is unique.

## Which One Should You Use?

| Situation | Best Measure |
|---|---|
| Normally distributed data, no outliers | Mean |
| Skewed data or outliers present | Median |
| Categorical data (Nominal/Ordinal) | Mode |
| Reporting income (often skewed by a few very high earners) | Median |
| Reporting exam scores (usually fairly even spread) | Mean |

## How This Connects to Day 4 (Levels of Measurement)

- **Nominal:** Only Mode makes sense (Mean/Median are meaningless for categories like gender codes)
- **Ordinal:** Median and Mode are appropriate (Mean is technically debated since distances are not equal)
- **Scale:** Mean, Median, and Mode are all valid, choose based on skewness

## Running This in SPSS

**Option A: Through Frequencies**
1. `Analyze` then `Descriptive Statistics` then `Frequencies`
2. Add your variable
3. Click `Statistics`
4. Check Mean, Median, Mode
5. Click Continue, then OK

**Option B: Through Descriptives (Mean only, faster for many variables)**
1. `Analyze` then `Descriptive Statistics` then `Descriptives`
2. Add your variable(s)
3. Click OK
(Note: Descriptives only gives Mean, not Median or Mode, we cover this fully with Std. Deviation on Day 7)

## Practice Task

Using your dataset from Day 3:

1. Run Mean, Median, and Mode for `age` and `monthly_income`
2. Compare the Mean and Median for `monthly_income`, if they are very different, that signals skewed data (a few high earners pulling the Mean up)
3. Write one sentence interpreting each result, for example: "The average monthly income was Rs. 45,000, but the median of Rs. 38,000 suggests the average is being pulled up by a small number of high earners."

## Key Takeaway

Never report the Mean blindly. Always check it against the Median, if they are far apart, your data is skewed and the Median is the more honest summary.
