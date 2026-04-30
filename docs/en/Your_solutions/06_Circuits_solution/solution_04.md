# Task 04 – Mixed Circuit

## Problem Statement

Calculate the equivalent resistance for a circuit where all resistors are $10\,\Omega$. (Assuming a "bridge" or "ladder" configuration: two parallel branches, each containing two resistors in series).

## Theory

For branches in parallel, we first calculate the resistance of each branch, then combine them.

## Step-by-Step Solution

1. **Calculate resistance of each series branch:**
   Branch A has two $10\,\Omega$ resistors in series:

$$
R_A = 10 + 10 = 20\,\Omega
$$

   Branch B has two $10\,\Omega$ resistors in series:

$$
R_B = 10 + 10 = 20\,\Omega
$$

2. **Calculate the parallel equivalent:**
   The two branches ($R_A$ and $R_B$) are in parallel.

$$
\begin{align}
\frac{1}{R_{eq}} &= \frac{1}{R_A} + \frac{1}{R_B} \\
&= \frac{1}{20} + \frac{1}{20} = \frac{2}{20}
\end{align}
$$

$$
R_{eq} = \frac{20}{2} = 10\,\Omega
$$

## Final Result

The total equivalent resistance is $10\,\Omega$.

## Interpretation

This specific configuration returns an equivalent resistance equal to a single resistor's value. This occurs because the doubling of resistance in the series branches is exactly balanced by the halving effect of the parallel connection.