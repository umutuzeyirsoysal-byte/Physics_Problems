# Task 11 – Dynamics with a Time-Dependent Force

## Problem Statement

A particle of mass $m=3\ \text{kg}$ moves in a force field dependent on time:

$$
\vec{F} = 
\begin{pmatrix}
15t \\
3t - 12 \\
-6t^2
\end{pmatrix}\ \text{N}
$$

Assuming initial conditions $\vec{r}_0 = \begin{pmatrix} 5 \\ 2 \\ -3 \end{pmatrix}\ \text{m}$ and $\vec{v}_0 = \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix}\ \text{m/s}$, find the position and velocity dependencies on time.

## Theory

Acceleration is found using Newton's Second Law. Velocity and position are found by successively integrating the acceleration vector with respect to time, applying the provided initial conditions to determine the constants of integration.

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

$$
\vec{v}(t) = \int \vec{a}(t) dt + \vec{v}_0
$$

$$
\vec{r}(t) = \int \vec{v}(t) dt + \vec{r}_0
$$

## Step-by-Step Solution

### 1. Acceleration

Divide the force vector by the mass $m=3$:

$$
\vec{a}(t) = 
\begin{pmatrix}
\frac{15t}{3} \\
\frac{3t - 12}{3} \\
\frac{-6t^2}{3}
\end{pmatrix}
=
\begin{pmatrix}
5t \\
t - 4 \\
-2t^2
\end{pmatrix}
$$

### 2. Velocity

Integrate the acceleration vector:

$$
\vec{v}(t) = 
\begin{pmatrix}
\int 5t \, dt \\
\int (t - 4) \, dt \\
\int -2t^2 \, dt
\end{pmatrix}
=
\begin{pmatrix}
2.5t^2 + C_x \\
0.5t^2 - 4t + C_y \\
-\frac{2}{3}t^3 + C_z
\end{pmatrix}
$$

Apply initial conditions $\vec{v}(0) = \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix}$:

$$
\begin{pmatrix}
C_x \\
C_y \\
C_z
\end{pmatrix}
=
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
$$

Thus, the velocity vector is:

$$
\vec{v}(t) = 
\begin{pmatrix}
2.5t^2 + 2 \\
0.5t^2 - 4t \\
-\frac{2}{3}t^3 + 1
\end{pmatrix}
$$

### 3. Position

Integrate the velocity vector:

$$
\vec{r}(t) = 
\begin{pmatrix}
\int (2.5t^2 + 2) \, dt \\
\int (0.5t^2 - 4t) \, dt \\
\int (-\frac{2}{3}t^3 + 1) \, dt
\end{pmatrix}
=
\begin{pmatrix}
\frac{2.5}{3}t^3 + 2t + D_x \\
\frac{0.5}{3}t^3 - 2t^2 + D_y \\
-\frac{2}{12}t^4 + t + D_z
\end{pmatrix}
$$

Apply initial conditions $\vec{r}(0) = \begin{pmatrix} 5 \\ 2 \\ -3 \end{pmatrix}$:

$$
\begin{pmatrix}
D_x \\
D_y \\
D_z
\end{pmatrix}
=
\begin{pmatrix}
5 \\
2 \\
-3
\end{pmatrix}
$$

Thus, the position vector is:

$$
\vec{r}(t) = 
\begin{pmatrix}
\frac{5}{6}t^3 + 2t + 5 \\
\frac{1}{6}t^3 - 2t^2 + 2 \\
-\frac{1}{6}t^4 + t - 3
\end{pmatrix}
$$

## Final Result

The time-dependent velocity and position vectors are:

$$
\vec{v}(t) = 
\begin{pmatrix}
2.5t^2 + 2 \\
0.5t^2 - 4t \\
-\frac{2}{3}t^3 + 1
\end{pmatrix}\ \text{m/s}
$$

$$
\vec{r}(t) = 
\begin{pmatrix}
\frac{5}{6}t^3 + 2t + 5 \\
\frac{1}{6}t^3 - 2t^2 + 2 \\
-\frac{1}{6}t^4 + t - 3
\end{pmatrix}\ \text{m}
$$

## Interpretation

Because the force varies polynomially with time, the resulting position vector terms climb in polynomial degree. The motion in the z-axis will dominate over long periods as it is governed by a higher power ($-t^4$) relative to the $t^3$ terms in the x and y axes.