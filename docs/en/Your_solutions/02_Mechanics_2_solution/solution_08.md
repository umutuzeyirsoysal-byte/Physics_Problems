# Task 08 – Work of a Variable Force

## Problem Statement

Given a one-dimensional force $F(x) = -kx$:
* Write down the equation of motion and solve it.
* Calculate the work done during the displacement from $0$ to $x_0$.
* Interpret the result as potential energy.
* Verify the relationship $F = -\frac{dU}{dx}$.
* Draw the graph of $F(x)$ and $U(x)$.

## Theory

Newton's Second Law gives the equation of motion. The definition of work for a variable 1D force is given by the integral:

$$
W = \int_{x_i}^{x_f} F(x) \, dx
$$

The work done by a conservative force is equal to the negative change in potential energy:

$$
W = -\Delta U
$$

## Step-by-Step Solution

### 1. Equation of Motion

From Newton's second law:

$$
m \frac{d^2 x}{dt^2} = -kx
$$

Rearranging yields the standard harmonic oscillator differential equation:

$$
\frac{d^2 x}{dt^2} + \frac{k}{m} x = 0
$$

Let $\omega = \sqrt{\frac{k}{m}}$. The general solution is:

$$
x(t) = A \cos(\omega t + \phi)
$$

where $A$ and $\phi$ are constants determined by initial conditions.

### 2. Work Done

The work done by the spring force from $0$ to $x_0$ is:

$$
\begin{align}
W &= \int_{0}^{x_0} (-kx) \, dx \\
  &= -k \left[ \frac{x^2}{2} \right]_{0}^{x_0} \\
  &= -\frac{1}{2} k x_0^2
\end{align}
$$

### 3. Interpretation as Potential Energy

Since the force is conservative, the work done equals the negative change in potential energy:

$$
W = -(U(x_0) - U(0))
$$

Setting the reference potential energy $U(0) = 0$, we get:

$$
-\frac{1}{2} k x_0^2 = -U(x_0)
$$

$$
U(x_0) = \frac{1}{2} k x_0^2
$$

This represents the elastic potential energy stored in the spring when displaced by $x_0$.

### 4. Verification of the Force-Potential Relationship

To verify the relationship $F = -\frac{dU}{dx}$, we take the derivative of the potential energy function $U(x) = \frac{1}{2}kx^2$:

$$
\begin{align}
-\frac{dU}{dx} &= -\frac{d}{dx} \left( \frac{1}{2} k x^2 \right) \\
               &= -\frac{1}{2} k (2x) \\
               &= -kx
\end{align}
$$

This matches the initial force $F(x) = -kx$.

### 5. Graphical Representation Description

* **Graph of $F(x)$:** A straight line passing through the origin with a negative slope equal to $-k$. It sits in the second and fourth quadrants.
* **Graph of $U(x)$:** A parabola opening upwards, with its vertex at the origin $(0,0)$. 

## Final Result

The motion equation is $x(t) = A \cos(\omega t + \phi)$. The work done is $W = -\frac{1}{2}kx_0^2$, which perfectly maps to the potential energy function $U(x) = \frac{1}{2}kx^2$, successfully verified via its spatial derivative.

## Interpretation

The negative sign in the work integral shows that the restoring force acts in the opposite direction of the displacement, removing kinetic energy from the system and storing it as elastic potential energy.