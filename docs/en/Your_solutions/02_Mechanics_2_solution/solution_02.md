# Task 02 – Harmonic Motion

## Problem Statement

A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). Determine the spring constant $k$ and the total mechanical energy of the system.

## Theory

The general equation for simple harmonic motion is

$$
x(t) = A \cos(\omega t + \phi)
$$

where $A$ is the amplitude and $\omega$ is the angular frequency. The angular frequency is related to the spring constant $k$ and mass $m$ by

$$
\omega = \sqrt{\frac{k}{m}}
$$

The total mechanical energy in a simple harmonic oscillator is conserved and given by

$$
E = \frac{1}{2} k A^2
$$

## Step-by-Step Solution

By comparing the given equation $x(t) = 0.2 \cos(10\pi t)$ with the general form, the amplitude and angular frequency are extracted:

$$
A = 0.2\ \text{m}
$$

$$
\omega = 10\pi\ \text{rad/s}
$$

Rearrange the angular frequency formula to solve for the spring constant $k$:

$$
k = m \omega^2
$$

Substitute the given mass $m = 10\ \text{kg}$ and $\omega$:

$$
k = 10 \cdot (10\pi)^2 = 10 \cdot 100\pi^2 = 1000\pi^2\ \text{N/m}
$$

Calculate the total mechanical energy using the formula:

$$
\begin{align}
E &= \frac{1}{2} k A^2 \\
  &= \frac{1}{2} (1000\pi^2) \cdot (0.2)^2 \\
  &= 500\pi^2 \cdot 0.04 \\
  &= 20\pi^2\ \text{J}
\end{align}
$$

For numerical approximations (using $\pi \approx 3.14159$):

$$
k \approx 1000 \cdot 9.8696 \approx 9870\ \text{N/m}
$$

$$
E \approx 20 \cdot 9.8696 \approx 197.4\ \text{J}
$$

## Final Result

The spring constant is $k = 1000\pi^2\ \text{N/m}$. The total mechanical energy is $E = 20\pi^2\ \text{J}$.

## Interpretation

The high spring constant indicates a very stiff spring, which explains the high frequency of oscillation ($5\ \text{Hz}$) despite a relatively large mass of $10\ \text{kg}$.