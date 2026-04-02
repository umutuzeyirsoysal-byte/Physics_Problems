# Task 03 – Conservation of Energy

## Problem Statement

A pendulum with a length of 1.0 meter is released from an initial angle of $15^\circ$. Calculate the speed of the pendulum bob at the bottom of its swing.

## Theory

By the principle of conservation of mechanical energy, the initial potential energy at the release point is entirely converted into kinetic energy at the lowest point of the trajectory. 

$$
E_i = E_f
$$

$$
mgh = \frac{1}{2} m v^2
$$

The height $h$ can be determined from the geometry of the pendulum:

$$
h = L - L\cos(\theta) = L(1 - \cos(\theta))
$$

## Step-by-Step Solution

Equating potential and kinetic energy:

$$
m g L (1 - \cos(\theta)) = \frac{1}{2} m v^2
$$

The mass $m$ cancels out from both sides:

$$
g L (1 - \cos(\theta)) = \frac{1}{2} v^2
$$

Solve for velocity $v$:

$$
v = \sqrt{2gL(1 - \cos(\theta))}
$$

Substitute the given values ($L = 1.0\ \text{m}$, $\theta = 15^\circ$, $g \approx 9.81\ \text{m/s}^2$):

$$
v = \sqrt{2 \cdot 9.81 \cdot 1.0 \cdot (1 - \cos(15^\circ))}
$$

Convert $15^\circ$ to evaluate the cosine ($\cos(15^\circ) \approx 0.9659$):

$$
\begin{align}
v &= \sqrt{19.62 \cdot (1 - 0.9659)} \\
  &= \sqrt{19.62 \cdot 0.0341} \\
  &\approx \sqrt{0.669} \\
  &\approx 0.818\ \text{m/s}
\end{align}
$$

## Final Result

The speed of the pendulum bob at the bottom of its swing is approximately $0.82\ \text{m/s}$.

## Interpretation

At such small angles, the vertical displacement $h$ is very small, leading to a modest velocity at the equilibrium position. The mass independence is a key feature of simple pendulum energy transfers.