# Task 07 – Standard Deviation

## Problem Statement

Given scores: 88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89. Calculate the mean ($\bar{x}$) and standard deviation ($\sigma$). Recalculate after removing the highest and lowest scores.

## Theory

The mean is:

$$
\bar{x} = \frac{1}{N} \sum_{i=1}^N x_i
$$

The sample standard deviation is:

$$
\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^N (x_i - \bar{x})^2}
$$

## Step-by-Step Solution

1. **Initial Set ($N=11$):**
   Sum $= 88+92+79+85+95+81+86+90+83+77+89 = 945$

$$
\bar{x} = \frac{945}{11} \approx 85.91
$$

   Calculating $\sum (x_i - \bar{x})^2$:
   $(2.09)^2 + (6.09)^2 + (-6.91)^2 + (-0.91)^2 + (9.09)^2 + (-4.91)^2 + (0.09)^2 + (4.09)^2 + (-2.91)^2 + (-8.91)^2 + (3.09)^2$
   $\approx 4.37 + 37.09 + 47.75 + 0.83 + 82.63 + 24.11 + 0.01 + 16.73 + 8.47 + 79.39 + 9.55 = 310.93$

$$
\sigma = \sqrt{\frac{310.93}{10}} \approx 5.58
$$

2. **Modified Set ($N=9$):**
   Remove lowest ($77$) and highest ($95$).
   New Sum $= 945 - 172 = 773$

$$
\bar{x}_{new} = \frac{773}{9} \approx 85.89
$$

   New $\sigma$:
   $\sum (x_i - \bar{x}_{new})^2 \approx 148.89$

$$
\sigma_{new} = \sqrt{\frac{148.89}{8}} \approx 4.31
$$

## Final Result

- **Original:** $\bar{x} \approx 85.91, \sigma \approx 5.58$
- **Modified:** $\bar{x} \approx 85.89, \sigma \approx 4.31$

## Interpretation

Removing outliers significantly reduces the standard deviation while the mean remains nearly the same, indicating the distribution is relatively symmetric but contains extreme values that inflate the spread.