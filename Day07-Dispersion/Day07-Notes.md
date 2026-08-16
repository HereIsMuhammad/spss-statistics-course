# Day 7: Measures of Dispersion (Range, Variance, Standard Deviation)

## Recap

On Day 6 we learned how to find the "center" of data using Mean, Median, and Mode. But two datasets can have the exact same Mean and still look completely different. Today we learn how to measure how spread out the data is.

## Why Dispersion Matters

**Example:** Two groups of exam scores, both with a Mean of 70:

- Group A: 68, 69, 70, 71, 72 (everyone scored close to 70)
- Group B: 20, 50, 70, 90, 120 (huge variation, but same average)

The Mean alone tells you nothing about this difference. You need a measure of spread to know if the data is tightly clustered or widely scattered.

## 1. Range

The simplest measure of spread, just the difference between the highest and lowest value.

**Formula:** Range = Maximum value − Minimum value

**Example:** Ages: 20, 22, 23, 25, 60
Range = 60 − 20 = 40

**Limitation:** The Range only looks at two extreme values, it ignores everything in between. One outlier can make the Range misleading.

## 2. Variance

Variance measures the average of the squared differences from the Mean. It shows how far, on average, each data point is from the center, but in squared units (which makes it hard to interpret directly).

**Why squared?** So that negative and positive differences from the Mean do not cancel each other out.

**Formula (simplified concept):**
Variance = Average of (each value − Mean)²

**Note:** Because it is squared, Variance is rarely reported directly in results, it is mainly a stepping stone to Standard Deviation.

## 3. Standard Deviation (SD)

Standard Deviation is the square root of Variance. This brings the number back into the same unit as your original data, making it much easier to interpret.

**Formula:** SD = √Variance

**How to interpret it:** SD tells you, on average, how far each data point is from the Mean.

- **Small SD** = data points are clustered close to the Mean (consistent, predictable)
- **Large SD** = data points are spread out widely (more variation, less consistent)

**Example:** If exam scores have a Mean of 70 and SD of 3, most students scored close to 70 (roughly 67 to 73). If the SD was 20 instead, scores would be all over the place (50 to 90), even though the Mean is the same.

## Quick Comparison Table

| Measure | What it Tells You | Sensitive to Outliers? |
|---|---|---|
| Range | Total spread (max to min) | Very sensitive |
| Variance | Average squared distance from Mean | Sensitive |
| Standard Deviation | Average distance from Mean, in original units | Sensitive |

## Reporting Mean with SD

In research, you will almost always see results reported as: **Mean = 70, SD = 3.2**

This single pairing tells the reader both the center AND the spread of the data, much more informative than the Mean alone.

## Running This in SPSS

1. `Analyze` then `Descriptive Statistics` then `Descriptives`
2. Move your Scale variable(s) into the box
3. Click `Options`
4. Check: Mean, Std. Deviation, Variance, Range, Minimum, Maximum
5. Click Continue, then OK

The Output table will show all selected statistics side by side for each variable.

## Practice Task

Using your dataset from Day 3:

1. Run Descriptives on `age` and `monthly_income`, include Range, Variance, and Standard Deviation
2. Compare the SD of `age` vs `monthly_income`, which one is more spread out relative to its Mean?
3. Write one sentence interpreting the SD, for example: "Monthly income had a high standard deviation (SD = 18,500) relative to its mean, indicating large income inequality among respondents."

## Key Takeaway

Never report a Mean alone. Always pair it with the Standard Deviation, this tells the full story: not just where the "center" is, but how much the data varies around it.
