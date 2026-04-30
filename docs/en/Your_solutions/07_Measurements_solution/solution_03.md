# Task 03 – Propagation of Error III

## Problem Statement

Calculate the resistance $R$ and its uncertainty given $V = (10.0 \pm 0.2)\text{ V}$ and $I = (2.00 \pm 0.05)\text{ A}$.

## Theory

Using Ohm's Law:

$$
R = \frac{V}{I}
$$

For a quotient, the relative uncertainty is:

$$
\frac{\Delta R}{R} = \sqrt{\left( \frac{\Delta V}{V} \right)^2 + \left( \frac{\Delta I}{I} \right)^2}
$$

## Step-by-Step Solution

1. **Calculate Resistance:**

$$
R = \frac{10.0}{2.00} = 5.00\,\Omega
$$

2. **Calculate Relative Uncertainty:**

$$
\frac{\Delta R}{R} = \sqrt{\left( \frac{0.2}{10.0} \right)^2 + \left( \frac{0.05}{2.00} \right)^2}
$$

$$
\frac{\Delta R}{R} = \sqrt{(0.02)^2 + (0.025)^2} = \sqrt{0.0004 + 0.000625} = 0.032\,\text{(3.2\%)}
$$

3. **Calculate Absolute Uncertainty:**

$$
\Delta R = 5.00 \cdot 0.032 = 0.16\,\Omega
$$

## Final Result

$$
R = (5.00 \pm 0.16)\,\Omega
$$

## Interpretation

The current measurement contributes slightly more to the final uncertainty ($2.5\%$) compared to the voltage measurement ($2\%$).