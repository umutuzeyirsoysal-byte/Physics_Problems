# Task 05 – Kirchhoff's Laws

## Problem Statement

Find the currents $I_1, I_2, I_3$ in a two-loop circuit:
- Left loop: $\mathcal{E}_1 = 4.5\,\text{V}$, $r_{w1} = 1\,\Omega$, $R_1 = 20\,\Omega$.
- Right loop: $\mathcal{E}_2 = 9\,\text{V}$, $r_{w2} = 1\,\Omega$.
- Shared branch: $R_2 = 10\,\Omega$.

## Theory

Kirchhoff's Current Law (KCL) states that the sum of currents entering a node equals the sum leaving it:

$$
\sum I_{in} = \sum I_{out}
$$

Kirchhoff's Voltage Law (KVL) states that the sum of voltages around any closed loop is zero:

$$
\sum V = 0
$$

## Step-by-Step Solution

Let $I_1$ be the current in the left branch, $I_3$ in the right branch, and $I_2$ in the shared middle branch. By KCL at the top node:

$$
I_1 + I_3 = I_2
$$

### Loop 1 (Left)
Clockwise from the bottom left:

$$
\mathcal{E}_1 - I_1(r_{w1} + R_1) - I_2 R_2 = 0
$$

$$
4.5 - 21I_1 - 10I_2 = 0
$$

### Loop 2 (Right)
Counter-clockwise from bottom right:

$$
\mathcal{E}_2 - I_3 r_{w2} - I_2 R_2 = 0
$$

$$
9 - 1I_3 - 10I_2 = 0
$$

### Solving the System
Substitute $I_2 = I_1 + I_3$ into the equations:

$$
\begin{align}
4.5 - 21I_1 - 10(I_1 + I_3) &= 0 \implies 31I_1 + 10I_3 = 4.5 \\
9 - I_3 - 10(I_1 + I_3) &= 0 \implies 10I_1 + 11I_3 = 9
\end{align}
$$

Solving for $I_3$ in the second equation: $11I_3 = 9 - 10I_1 \implies I_3 = \frac{9 - 10I_1}{11}$.
Substitute into the first:

$$
31I_1 + 10\left(\frac{9 - 10I_1}{11}\right) = 4.5
$$

Multiply by 11:

$$
341I_1 + 90 - 100I_1 = 49.5
$$

$$
241I_1 = -40.5 \implies I_1 \approx -0.168\,\text{A}
$$

Using $I_1$ to find $I_3$:

$$
I_3 = \frac{9 - 10(-0.168)}{11} \approx 0.971\,\text{A}
$$

Finally, $I_2$:

$$
I_2 = -0.168 + 0.971 = 0.803\,\text{A}
$$

## Final Result

- $I_1 \approx -0.168\,\text{A}$ (current flows opposite to assumed direction)
- $I_2 \approx 0.803\,\text{A}$
- $I_3 \approx 0.971\,\text{A}$

## Interpretation

The negative value for $I_1$ indicates that the $9\,\text{V}$ source is dominant, actually forcing current backwards through the $4.5\,\text{V}$ source branch.