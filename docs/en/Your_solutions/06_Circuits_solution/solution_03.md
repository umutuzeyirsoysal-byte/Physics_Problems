# Task 03 – Mixed Circuit

## Problem Statement

Calculate the equivalent resistance for a mixed circuit where all resistors have a resistance of $R = 5\,\Omega$. (Assuming a standard configuration: two resistors in parallel, connected in series with a third resistor).

## Theory

To solve mixed circuits, identify portions of the circuit that are purely in series or purely in parallel. Replace them with their equivalent resistance and simplify the circuit step-by-step.

- Parallel: $R_p = \left( \frac{1}{R_1} + \frac{1}{R_2} \right)^{-1}$
- Series: $R_s = R_1 + R_2$

## Step-by-Step Solution

1. **Analyze the parallel branch:**
   Two $5\,\Omega$ resistors are in parallel.

$$
R_{parallel} = \frac{R \cdot R}{R + R} = \frac{5 \cdot 5}{5 + 5} = \frac{25}{10} = 2.5\,\Omega
$$

2. **Add the series component:**
   This parallel block is in series with the third $5\,\Omega$ resistor.

$$
R_{eq} = R_{parallel} + R_3 = 2.5\,\Omega + 5\,\Omega = 7.5\,\Omega
$$

## Final Result

The equivalent resistance of the circuit is $7.5\,\Omega$.

## Interpretation

In mixed circuits, parallel branches reduce the total resistance relative to a simple series circuit, but the series components ensure the total resistance remains higher than the parallel section alone.