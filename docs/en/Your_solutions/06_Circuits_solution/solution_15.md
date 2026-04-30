# Task 15 – Resistor Cube

## Problem Statement

A cube is constructed from 12 identical resistors $R$. Calculate the equivalent resistance between two opposite corners.

## Theory

Due to the symmetry of the cube, we can use the concept of equipotential nodes. If we apply a potential difference between opposite corners, nodes equidistant from the start/end points must be at the same potential.

## Step-by-Step Solution

Let the input corner be $A$ and the opposite corner be $B$. 

1. **Step 1: From corner A.** There are 3 edges leaving A. Due to symmetry, the current $I$ divides equally into $I/3$ through each resistor.
2. **Step 2: Intermediate nodes.** Each of these 3 currents reaches a node where it splits into 2 edges. There are 6 such edges in the middle of the cube, each carrying $(I/3) / 2 = I/6$.
3. **Step 3: To corner B.** The 6 middle paths converge into 3 resistors that meet at corner B. Each carries $I/3$.

The total voltage drop $V$ is the sum of drops along any path from A to B:

$$
\begin{align}
V &= V_1 + V_2 + V_3 \\
&= \left( \frac{I}{3} \right) R + \left( \frac{I}{6} \right) R + \left( \frac{I}{3} \right) R
\end{align}
$$

Factoring out $IR$:

$$
V = IR \left( \frac{2}{6} + \frac{1}{6} + \frac{2}{6} \right) = IR \left( \frac{5}{6} \right)
$$

Since $R_{eq} = V/I$:

$$
R_{eq} = \frac{5}{6} R
$$

## Final Result

The equivalent resistance is $\frac{5}{6} R$.

## Interpretation

Symmetry significantly simplifies complex network problems. By identifying nodes with equal potential, we can treat the circuit as a series of parallel-connected groups.