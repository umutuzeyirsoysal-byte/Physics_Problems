# Task 02 – Resistors

## Problem Statement

Given exactly three $1\,\Omega$ resistors, determine all possible unique equivalent resistances that can be created by combining them.

## Theory

Resistors can be combined in series, parallel, or mixed configurations.
- Series: $R_{eq} = R_1 + R_2 + \dots$
- Parallel: $R_{eq} = (R_1^{-1} + R_2^{-1} + \dots)^{-1}$

## Step-by-Step Solution

1. **All in series:**
   
$$
R = 1 + 1 + 1 = 3\,\Omega
$$

2. **All in parallel:**
   
$$
\frac{1}{R} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 3 \implies R = \frac{1}{3}\,\Omega \approx 0.33\,\Omega
$$

3. **Two in series, one in parallel to the pair:**
   
$$
\frac{1}{R} = \frac{1}{1+1} + \frac{1}{1} = \frac{1}{2} + 1 = \frac{3}{2} \implies R = \frac{2}{3}\,\Omega \approx 0.67\,\Omega
$$

4. **Two in parallel, one in series to the pair:**
   
$$
R = \left(\frac{1}{1} + \frac{1}{1}\right)^{-1} + 1 = 0.5 + 1 = 1.5\,\Omega
$$

5. **Single resistor or other subsets:** The problem specifies "using three resistors," but if subsets are excluded, the four values above are the only unique combinations using all three.

## Final Result

The unique equivalent resistances are: $3\,\Omega$, $1.5\,\Omega$, $0.67\,\Omega$, and $0.33\,\Omega$.

## Interpretation

The maximum resistance is achieved by connecting all components in series, while the minimum is achieved by connecting all in parallel. Mixed circuits provide intermediate values.