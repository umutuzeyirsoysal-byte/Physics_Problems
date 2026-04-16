# Task 03 – Electrostatic Equilibrium

## Problem Statement

Find the equilibrium position for a charge $q_3 = +1\text{C}$ placed on the line between a charge $q_1 = +4\text{C}$ and a charge $q_2 = +9\text{C}$, which are separated by a distance of 2 m.

## Theory

A charge is in **electrostatic equilibrium** when the net electric force acting on it is zero:

$$
\sum \vec{F} = 0
$$

For a third charge placed between two positive charges, the forces exerted by $q_1$ and $q_2$ will point in opposite directions. Equilibrium occurs where the magnitudes of these two forces are equal:

$$
F_1 = F_2
$$

## Step-by-Step Solution

### 1. Setup the Coordinate System
Let $q_1$ be at $x = 0$ and $q_2$ be at $x = L = 2\text{ m}$.
Place $q_3$ at an unknown distance $x$ from $q_1$. The distance from $q_3$ to $q_2$ is therefore $L - x$.

### 2. Set the Forces Equal
Using Coulomb's Law:

$$
k_e \frac{q_1 q_3}{x^2} = k_e \frac{q_2 q_3}{(L - x)^2}
$$

Cancel $k_e$ and $q_3$ from both sides:

$$
\frac{q_1}{x^2} = \frac{q_2}{(L - x)^2}
$$

### 3. Solve for x
Substitute the given values $q_1 = 4$ and $q_2 = 9$:

$$
\frac{4}{x^2} = \frac{9}{(2 - x)^2}
$$

Take the square root of both sides to simplify:

$$
\frac{2}{x} = \frac{3}{2 - x}
$$

Cross-multiply:

$$
2(2 - x) = 3x
$$

$$
4 - 2x = 3x
$$

$$
4 = 5x \implies x = 0.8\text{ m}
$$

## Final Result

The equilibrium position is $0.8\text{ m}$ from the charge $q_1 = +4\text{C}$ (or $1.2\text{ m}$ from $q_2$).

## Interpretation

The equilibrium point is closer to the smaller charge ($q_1$), which is physically intuitive