# Task 01 – Coulomb's Law

## Problem Statement

Four point charges of $+1.0\text{ C}$ each are placed at the corners of a square with sides of $1.0\text{ m}$. Calculate the magnitude and direction of the electric force on a charge of $-2.0\text{ C}$ placed at the center of the square.

## Theory

According to **Coulomb's Law**, the magnitude of the electrostatic force between two point charges $q_1$ and $q_2$ separated by a distance $r$ is given by

$$
F = k_e \frac{|q_1 q_2|}{r^2}
$$

where $k_e \approx 8.99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$ is Coulomb's constant.

The **Principle of Superposition** states that the total force acting on a charge is the vector sum of the individual forces exerted by all other charges in the system:

$$
\vec{F}_{net} = \sum_{i=1}^{n} \vec{F}_i
$$

## Step-by-Step Solution

### 1. Geometry of the System
Place the square in the $xy$-plane. The side length is $s = 1.0\text{ m}$.
The distance from a corner to the center of a square is half the diagonal $d$.

$$
d = \sqrt{s^2 + s^2} = s\sqrt{2} = \sqrt{2}\text{ m}
$$

The distance $r$ from each corner charge to the center charge is:

$$
r = \frac{d}{2} = \frac{\sqrt{2}}{2}\text{ m}
$$

### 2. Analysis of Force Vectors
Let the four corner charges be $Q_1, Q_2, Q_3, Q_4$, where $Q_i = +1.0\text{ C}$.
Let the center charge be $q = -2.0\text{ C}$.

Since all corner charges are identical and equidistant from the center, the magnitude of the force exerted by any single corner charge on the center charge is:

$$
F_i = k_e \frac{|Q_i q|}{r^2}
$$

Substituting the values:

$$
F_i = k_e \frac{|(1.0)( -2.0)|}{(\sqrt{2}/2)^2} = k_e \frac{2}{2/4} = 4k_e
$$

### 3. Vector Summation
Consider the diagonal pairs.
- The force from the top-left charge points toward the top-left corner (attractive).
- The force from the bottom-right charge points toward the bottom-right corner (attractive).

Because these two charges are equal and located at opposite ends of a diagonal passing through the center, their force vectors are equal in magnitude but opposite in direction:

$$
\vec{F}_{top-left} + \vec{F}_{bottom-right} = \vec{0}
$$

The same logic applies to the other diagonal:

$$
\vec{F}_{top-right} + \vec{F}_{bottom-left} = \vec{0}
$$

## Final Result

The net electric force is:

$$
\vec{F}_{net} = \vec{0}\text{ N}
$$

## Interpretation

The symmetry of the charge distribution results in a complete cancellation of the force vectors. Any test charge placed at the geometric center of a symmetric distribution of identical charges will experience a net force of zero, as the components in every direction are balanced by an equal and