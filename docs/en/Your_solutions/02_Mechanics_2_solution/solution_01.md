# Task 01 – Gravitational Dependence

## Problem Statement

A simple pendulum has a period of 4 seconds on Earth. Determine its period on the Moon, where the gravitational acceleration is about 1/6th of Earth's. Additionally, find the required length of a simple pendulum to have a period of exactly 1 second on Earth.

## Theory

The period of a simple pendulum for small angle oscillations is given by

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

where $L$ is the length of the pendulum and $g$ is the acceleration due to gravity. The period is independent of the mass of the pendulum bob.

## Step-by-Step Solution

### Part 1: Period on the Moon

Let $T_E$ be the period on Earth and $T_M$ be the period on the Moon. The gravitational acceleration on the Moon is

$$
g_M = \frac{g_E}{6}
$$

The period on Earth is

$$
T_E = 2\pi \sqrt{\frac{L}{g_E}} = 4\ \text{s}
$$

The period on the Moon is

$$
T_M = 2\pi \sqrt{\frac{L}{g_M}}
$$

Substitute $g_M$:

$$
\begin{align}
T_M &= 2\pi \sqrt{\frac{L}{\frac{g_E}{6}}} \\
    &= \sqrt{6} \cdot 2\pi \sqrt{\frac{L}{g_E}} \\
    &= \sqrt{6} \cdot T_E
\end{align}
$$

Calculate the numerical value:

$$
T_M = 4 \cdot \sqrt{6} \approx 4 \cdot 2.449 \approx 9.80\ \text{s}
$$

### Part 2: Required Length for a 1-Second Period on Earth

Rearrange the period formula to solve for $L$:

$$
L = g_E \left( \frac{T}{2\pi} \right)^2
$$

Substitute $T = 1\ \text{s}$ and $g_E \approx 9.81\ \text{m/s}^2$:

$$
L = 9.81 \cdot \left( \frac{1}{2\pi} \right)^2 \approx \frac{9.81}{39.48} \approx 0.248\ \text{m}
$$

## Final Result

The period on the Moon would be approximately $9.80\ \text{s}$. The required length for a 1-second period on Earth is approximately $0.248\ \text{m}$ (or $24.8\ \text{cm}$).

## Interpretation

A lower gravitational acceleration leads to a lower restoring force for the pendulum, increasing the time required to complete one full oscillation. A "seconds pendulum" (which ticks every half period) requires a length of nearly a quarter of a meter.