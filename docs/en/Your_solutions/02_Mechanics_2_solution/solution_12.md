# Task 12 – Work and Energy with a Constant Force

## Problem Statement

A constant force acts on a body of mass $m = 2\ \text{kg}$: $\vec{F} = \begin{pmatrix} 6 \\ 2 \end{pmatrix}\ \text{N}$. The body starts with velocity $\vec{v}(0) = \begin{pmatrix} 1 \\ -1 \end{pmatrix}\ \text{m/s}$ from $\vec{r}(0) = \begin{pmatrix} 0 \\ 0 \end{pmatrix}\ \text{m}$.
* Determine $\vec{a}(t)$, $\vec{v}(t)$, $\vec{r}(t)$.
* Draw the trajectory of the motion.
* Calculate the work done by the force at time $t=3\ \text{s}$.
* Check the consistency with the work-energy theorem.

## Theory

For a constant force, the acceleration is constant. Kinematics equations yield:

$$
\vec{v}(t) = \vec{a}t + \vec{v}_0
$$

$$
\vec{r}(t) = \frac{1}{2}\vec{a}t^2 + \vec{v}_0 t + \vec{r}_0
$$

Work done by a constant force is the dot product of force and displacement:

$$
W = \vec{F} \cdot \Delta\vec{r}
$$

The Work-Energy Theorem states that the work done equals the change in kinetic energy:

$$
W = \Delta E_k = \frac{1}{2} m v_f^2 - \frac{1}{2} m v_i^2
$$

## Step-by-Step Solution

### 1. Kinematics

Calculate acceleration $\vec{a} = \frac{\vec{F}}{m}$:

$$
\vec{a} = \frac{1}{2} 
\begin{pmatrix}
6 \\
2
\end{pmatrix}
=
\begin{pmatrix}
3 \\
1
\end{pmatrix}\ \text{m/s}^2
$$

Calculate velocity $\vec{v}(t)$:

$$
\vec{v}(t) = 
\begin{pmatrix}
3 \\
1
\end{pmatrix} t
+
\begin{pmatrix}
1 \\
-1
\end{pmatrix}
=
\begin{pmatrix}
3t + 1 \\
t - 1
\end{pmatrix}\ \text{m/s}
$$

Calculate position $\vec{r}(t)$:

$$
\vec{r}(t) = 
\frac{1}{2} 
\begin{pmatrix}
3 \\
1
\end{pmatrix} t^2
+
\begin{pmatrix}
1 \\
-1
\end{pmatrix} t
=
\begin{pmatrix}
1.5t^2 + t \\
0.5t^2 - t
\end{pmatrix}\ \text{m}
$$

### 2. Trajectory Description

By isolating $t$ from the equations of $x(t)$ and $y(t)$, one would find an equation describing a parabola. In the spatial $(x, y)$ coordinate system, the particle outlines a parabolic path, opening outwards towards the positive x and y quadrants.

### 3. Work Done at $t=3\ \text{s}$

Evaluate displacement at $t=3$:

$$
\vec{r}(3) = 
\begin{pmatrix}
1.5(3)^2 + 3 \\
0.5(3)^2 - 3
\end{pmatrix}
=
\begin{pmatrix}
1.5(9) + 3 \\
0.5(9) - 3
\end{pmatrix}
=
\begin{pmatrix}
16.5 \\
1.5
\end{pmatrix}\ \text{m}
$$

Since $\vec{r}(0) = (0, 0)$, the displacement vector is $\Delta\vec{r} = \begin{pmatrix} 16.5 \\ 1.5 \end{pmatrix}$. Calculate work $W$:

$$
\begin{align}
W &= \vec{F} \cdot \Delta\vec{r} \\
  &= 6(16.5) + 2(1.5) \\
  &= 99 + 3 \\
  &= 102\ \text{J}
\end{align}
$$

### 4. Work-Energy Theorem Check

Find initial speed squared $v(0)^2$:

$$
v_0^2 = 1^2 + (-1)^2 = 2\ \text{(m/s)}^2
$$

Find final velocity at $t=3$:

$$
\vec{v}(3) = 
\begin{pmatrix}
3(3) + 1 \\
3 - 1
\end{pmatrix}
=
\begin{pmatrix}
10 \\
2
\end{pmatrix}\ \text{m/s}
$$

Find final speed squared $v(3)^2$:

$$
v_f^2 = 10^2 + 2^2 = 100 + 4 = 104\ \text{(m/s)}^2
$$

Calculate change in kinetic energy:

$$
\begin{align}
\Delta E_k &= \frac{1}{2} m v_f^2 - \frac{1}{2} m v_0^2 \\
           &= \frac{1}{2} (2) (104) - \frac{1}{2} (2) (2) \\
           &= 104 - 2 \\
           &= 102\ \text{J}
\end{align}
$$

## Final Result

The kinematic equations strictly follow constant acceleration models. The work calculated by integrating force over distance yields $102\ \text{J}$. This identically equals the $102\ \text{J}$ increase in kinetic energy, confirming the work-energy theorem.

## Interpretation

Despite the initial velocity partially opposing the force direction in the y-axis, the overall motion ultimately aligns with the applied force. The equivalence of both approaches demonstrates that energy formalisms hold perfectly true in vector kinematic frameworks.