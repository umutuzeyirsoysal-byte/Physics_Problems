# Task 02 – Electric Potential

## Problem Statement

Point charges of $+1\text{C}$, $-2\text{C}$, $+3\text{C}$, and $-4\text{C}$ are placed at the corners of a square with sides of $1.0\text{ m}$ (in order). Calculate the electric potential at the center of the square.

## Theory

The electric potential $V$ at a distance $r$ from a point charge $q$ is a scalar quantity defined as:

$$
V = k_e \frac{q}{r}
$$

For a system of $n$ point charges, the total potential at a point is the algebraic sum of the potentials created by each charge:

$$
V_{total} = \sum_{i=1}^{n} k_e \frac{q_i}{r_i}
$$

Unlike force, potential is a scalar, so we do not need to consider directions, only the signs of the charges.

## Step-by-Step Solution

### 1. Determine the Distance
As calculated in Task 1, for a square of side $s = 1.0\text{ m}$, the distance $r$ from each corner to the center is:

$$
r = \frac{s\sqrt{2}}{2} = \frac{\sqrt{2}}{2}\text{ m}
$$

### 2. Summation of Potentials
The charges are $q_1 = +1$, $q_2 = -2$, $q_3 = +3$, and $q_4 = -4$ (all in Coulombs).
Since $r$ is common to all charges, we can factor the expression:

$$
V_{center} = \frac{k_e}{r} \sum q_i
$$

$$
V_{center} = \frac{k_e}{\sqrt{2}/2} (1 - 2 + 3 - 4)
$$

### 3. Numerical Calculation
Simplify the sum of charges:

$$
\sum q_i = 1 - 2 + 3 - 4 = -2\text{ C}
$$

Substitute back into the potential formula:

$$
V_{center} = \frac{2k_e}{\sqrt{2}} (-2) = -2\sqrt{2} k_e
$$

Using $k_e \approx 8.99 \times 10^9\text{ V}\cdot\text{m}/\text{C}$:

$$
V_{center} \approx -2 \cdot 1.414 \cdot 8.99 \times 10^9
$$

$$
V_{center} \approx -2.54 \times 10^{10}\text{ V}
$$

## Final Result

The electric potential at the center is:

$$
V = -2\sqrt{2} k_e \approx -2.54 \times 10^{10}\text{ V}
$$

## Interpretation

The negative result indicates that the net work required to bring a positive test charge from infinity to the center of the square is negative. In other words, the configuration is dominated by the negative charges in terms of potential energy at that specific point.