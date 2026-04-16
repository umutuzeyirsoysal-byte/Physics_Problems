# Task 06 – Field from a System of Charges

## Problem Statement

Two point charges are given: $+q$ at $(-a, 0)$ and $+2q$ at $(a, 0)$.
1. Determine the field vectors $\vec{E}(0, y)$, $\vec{E}(x, 0)$, and $\vec{E}(x, y)$.
2. Determine conditions for $E_x = 0$, $E_y = 0$, and $\vec{E} = 0$.
3. Calculate the field for $a = 0.2\text{ m}, y = 0.3\text{ m}, q = 2\mu\text{C}$.
4. Investigate the limit $y \gg a$.

## Theory

The electric field $\vec{E}$ at a point $\vec{r}$ due to a charge $q_i$ at $\vec{r}_i$ is:

$$
\vec{E}_i = \frac{k_e q_i}{|\vec{r} - \vec{r}_i|^3} (\vec{r} - \vec{r}_i)
$$

## Step-by-Step Solution

### 1. General Field Vector $\vec{E}(x, y)$
Charge 1: $q_1 = q$ at $\vec{r}_1 = (-a, 0)$.
Charge 2: $q_2 = 2q$ at $\vec{r}_2 = (a, 0)$.

$$
\vec{E}(x, y) = k_e q \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} + \frac{2((x-a)\hat{i} + y\hat{j})}{((x-a)^2 + y^2)^{3/2}} \right]
$$

**Specific cases:**
- **On the x-axis ($y=0$):**
$$
\vec{E}(x, 0) = k_e q \left[ \frac{x+a}{|x+a|^3} + \frac{2(x-a)}{|x-a|^3} \right] \hat{i}
$$
- **On the y-axis ($x=0$):**
$$
\vec{E}(0, y) = k_e q \left[ \frac{a\hat{i} + y\hat{j}}{(a^2 + y^2)^{3/2}} + \frac{-2a\hat{i} + 2y\hat{j}}{(a^2 + y^2)^{3/2}} \right] = \frac{k_e q}{(a^2 + y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})
$$

### 2. Conditions for Zero Field
- $E_y = 0$: Occurs when $y=0$ (on the x-axis).
- $E_x = 0$: On the y-axis, this never happens except at infinity. In general space, it requires the horizontal components to cancel.
- $\vec{E} = 0$: Must be on the x-axis between the charges. Set $E(x, 0) = 0$ for $-a < x < a$:
$$
\frac{1}{(x+a)^2} = \frac{2}{(a-x)^2} \implies \frac{a-x}{x+a} = \sqrt{2}
$$
Solving for $x$: $x = a\frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.17a$.

### 3. Numerical Calculation
For $a = 0.2, y = 0.3, x = 0, q = 2 \times 10^{-6}$:
$r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.36\text{ m}$.

$$
\vec{E}(0, 0.3) = \frac{(8.99 \times 10^9)(2 \times 10^{-6})}{(0.13)^{3/2}} (-0.2\hat{i} + 0.9\hat{j})
$$

### 4. Limit $y \gg a$
When $y \gg a$, $(a^2 + y^2)^{3/2} \approx y^3$.
$$
\vec{E}(0, y) \approx \frac{k_e q}{y^3} (-a\hat{i} + 3y\hat{j}) \approx \frac{3k_e q}{y^2}\hat{j}
$$
This simplifies to the field of a single charge $3q$ at the origin.

## Final Result
The field at $(0, y)$ is:
$$
\vec{E}(0, y) = \frac{k_e q}{(a^2 + y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})
$$

## Interpretation
At large distances, the system behaves like a point charge equal to the sum of the charges ($3q$). Near the charges, the asymmetry ($q$ vs $2q$) shifts the equilibrium point toward the weaker charge.