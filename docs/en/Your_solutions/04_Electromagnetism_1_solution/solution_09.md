# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with a velocity $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k})\text{ m/s}$ in a region where the magnetic field is $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k})\text{ T}$. What is the magnitude of the magnetic force this charge experiences?

## Theory

The magnetic force vector is calculated using the cross product:

$$
\vec{F} = q(\vec{v} \times \vec{B})
$$

For a proton, $q = e \approx 1.6 \times 10^{-19}\text{ C}$.

## Step-by-Step Solution

### 1. Calculate the Cross Product
Using the determinant method for $\vec{v} \times \vec{B}$:

$$
\vec{v} \times \vec{B} = 
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

$$
\vec{v} \times \vec{B} = [(-4)(-1) - (1)(2)]\hat{i} - [(2)(-1) - (1)(1)]\hat{j} + [(2)(2) - (-4)(1)]\hat{k}
$$

$$
\vec{v} \times \vec{B} = (4 - 2)\hat{i} - (-2 - 1)\hat{j} + (4 + 4)\hat{k} = 2\hat{i} + 3\hat{j} + 8\hat{k}
$$

### 2. Find the Magnitude of the Cross Product

$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2} = \sqrt{4 + 9 + 64} = \sqrt{77} \approx 8.775
$$

### 3. Calculate Force Magnitude

$$
F = q |\vec{v} \times \vec{B}| = (1.6 \times 10^{-19})(8.775) \approx 1.4 \times 10^{-18}\text{ N}
$$

## Final Result

The magnitude of the magnetic force is approximately $1.4 \times 10^{-18}\text{ N}$.

## Interpretation
The force is perpendicular to both the velocity and the magnetic field vectors. In vector form, $\vec{F} \approx (3.2\hat{i} + 4.8\hat{j} + 12.8\hat{k}) \times 10^{-19}\text{ N}$.