# Task 01 – Series and Parallel Circuits

## Problem Statement

Three resistors $R_1 = 15\,\Omega$, $R_2 = 30\,\Omega$, and $R_3 = 50\,\Omega$ are connected to a $12\,\text{V}$ battery. Calculate the total equivalent resistance and the current flowing from the battery for:
1. All resistors in series.
2. All resistors in parallel.

## Theory

For resistors in series, the equivalent resistance $R_{eq}$ is the sum of individual resistances:

$$
R_{eq} = \sum_{i=1}^{n} R_i
$$

For resistors in parallel, the reciprocal of the equivalent resistance is the sum of the reciprocals:

$$
\frac{1}{R_{eq}} = \sum_{i=1}^{n} \frac{1}{R_i}
$$

According to Ohm's Law, the total current $I$ is:

$$
I = \frac{V}{R_{eq}}
$$

## Step-by-Step Solution

### Case 1: Series Connection

The equivalent resistance is:

$$
R_{eq,s} = R_1 + R_2 + R_3 = 15\,\Omega + 30\,\Omega + 50\,\Omega = 95\,\Omega
$$

The total current is:

$$
I_s = \frac{12\,\text{V}}{95\,\Omega} \approx 0.126\,\text{A}
$$

### Case 2: Parallel Connection

The equivalent resistance is:

$$
\frac{1}{R_{eq,p}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}
$$

Finding a common denominator ($150$):

$$
\begin{align}
\frac{1}{R_{eq,p}} &= \frac{10}{150} + \frac{5}{150} + \frac{3}{150} \\
&= \frac{18}{150}
\end{align}
$$

Thus:

$$
R_{eq,p} = \frac{150}{18} \approx 8.33\,\Omega
$$

The total current is:

$$
I_p = \frac{12\,\text{V}}{8.333\,\Omega} = 1.44\,\text{A}
$$

## Final Result

- **Series:** $R_{eq} = 95\,\Omega$, $I = 0.126\,\text{A}$
- **Parallel:** $R_{eq} \approx 8.33\,\Omega$, $I = 1.44\,\text{A}$

## Interpretation

In a series circuit, resistance adds up, leading to a higher total resistance and lower current. In a parallel circuit, the total resistance is always less than the smallest individual resistor, resulting in a higher total current from the source.