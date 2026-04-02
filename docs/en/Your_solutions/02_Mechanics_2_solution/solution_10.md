# Task 10 – Force Field and Power

## Problem Statement

In a certain force field, the equations of motion of a particle with mass $m=0.5\ \text{kg}$ are given by:

$$
x(t) = 5t^2 - t, \quad y(t) = 2t^3, \quad z(t) = -3t + 2
$$

Find the time dependence of: the particle's velocity, the particle's momentum, the particle's acceleration, the force acting on the particle, and the power transferred by the field to the particle.

## Theory

The kinematic quantities are found by taking successive time derivatives of the position vector $\vec{r}(t)$.

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

Dynamic quantities depend on the particle's mass $m$. Linear momentum is the product of mass and velocity.

$$
\vec{p}(t) = m\vec{v}(t)
$$

By Newton's Second Law, the net force is the product of mass and acceleration.

$$
\vec{F}(t) = m\vec{a}(t)
$$

Mechanical power is defined as the rate at which work is done, which can be computed as the dot product of the force and velocity vectors.

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t)
$$

## Step-by-Step Solution

### 1. Velocity

The position vector is:

$$
\vec{r}(t) = 
\begin{pmatrix}
5t^2 - t \\
2t^3 \\
-3t + 2
\end{pmatrix}
$$

Taking the first derivative with respect to time yields the velocity:

$$
\vec{v}(t) = 
\begin{pmatrix}
\frac{d}{dt}(5t^2 - t) \\
\frac{d}{dt}(2t^3) \\
\frac{d}{dt}(-3t + 2)
\end{pmatrix}
=
\begin{pmatrix}
10t - 1 \\
6t^2 \\
-3
\end{pmatrix}
$$

### 2. Momentum

Multiply the velocity vector by the mass $m = 0.5\ \text{kg}$:

$$
\vec{p}(t) = 0.5 \cdot
\begin{pmatrix}
10t - 1 \\
6t^2 \\
-3
\end{pmatrix}
=
\begin{pmatrix}
5t - 0.5 \\
3t^2 \\
-1.5
\end{pmatrix}
$$

### 3. Acceleration

Taking the derivative of the velocity vector yields the acceleration:

$$
\vec{a}(t) = 
\begin{pmatrix}
\frac{d}{dt}(10t - 1) \\
\frac{d}{dt}(6t^2) \\
\frac{d}{dt}(-3)
\end{pmatrix}
=
\begin{pmatrix}
10 \\
12t \\
0
\end{pmatrix}
$$

### 4. Force

Multiply the acceleration vector by the mass $m = 0.5\ \text{kg}$:

$$
\vec{F}(t) = 0.5 \cdot
\begin{pmatrix}
10 \\
12t \\
0
\end{pmatrix}
=
\begin{pmatrix}
5 \\
6t \\
0
\end{pmatrix}
$$

### 5. Power

Compute the dot product of the force and velocity vectors:

$$
\begin{align}
P(t) &= F_x v_x + F_y v_y + F_z v_z \\
     &= (5)(10t - 1) + (6t)(6t^2) + (0)(-3) \\
     &= 50t - 5 + 36t^3
\end{align}
$$

Rearranging into descending powers of $t$:

$$
P(t) = 36t^3 + 50t - 5
$$

## Final Result

The required quantities as functions of time are:

$$
\vec{v}(t) = 
\begin{pmatrix}
10t - 1 \\
6t^2 \\
-3
\end{pmatrix}\ \text{m/s}
$$

$$
\vec{p}(t) = 
\begin{pmatrix}
5t - 0.5 \\
3t^2 \\
-1.5
\end{pmatrix}\ \text{kg m/s}
$$

$$
\vec{a}(t) = 
\begin{pmatrix}
10 \\
12t \\
0
\end{pmatrix}\ \text{m/s}^2
$$

$$
\vec{F}(t) = 
\begin{pmatrix}
5 \\
6t \\
0
\end{pmatrix}\ \text{N}
$$

$$
P(t) = 36t^3 + 50t - 5\ \text{W}
$$

## Interpretation

The particle experiences a constant driving force along the x-axis and a linearly increasing force along the y-axis, while coasting at a constant velocity along the z-axis (zero net force). Because the force in the y-direction scales with $t$ and acts on a velocity that scales with $t^2$, the total power transferred to the particle grows cubically over time.