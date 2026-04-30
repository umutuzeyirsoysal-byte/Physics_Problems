# Task 09 – Pendulum Measurements

## Problem Statement

Use a pendulum simulator to perform $10$ measurements of $10$ oscillations. Calculate the mean period, standard deviation, and the acceleration due to gravity $g$ with its uncertainty.

## Theory

The period of a simple pendulum is:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Solving for $g$:

$$
g = \frac{4\pi^2 L}{T^2}
$$

Uncertainty in $g$ (assuming $L$ is exact):

$$
\Delta g = g \cdot \left( 2 \frac{\Delta T}{T} \right)
$$

## Step-by-Step Solution

### 1. Data Collection
(Simulated data for $L = 1.0\,\text{m}$):
Times for $10T$: $20.1, 20.0, 20.2, 20.1, 19.9, 20.1, 20.3, 20.0, 20.1, 20.2$ (seconds).

### 2. Mean Period

$$
\bar{t}_{10} = 20.1\,\text{s} \implies \bar{T} = 2.01\,\text{s}
$$

### 3. Standard Deviation
Based on the variation: $\sigma_T \approx 0.012\,\text{s}$.

### 4. Calculate $g$

$$
g = \frac{4\pi^2 (1.0)}{(2.01)^2} \approx \frac{39.478}{4.0401} \approx 9.77\,\text{m/s}^2
$$

### 5. Uncertainty in $g$

$$
\Delta g = 9.77 \cdot \left( 2 \cdot \frac{0.012}{2.01} \right) \approx 0.12\,\text{m/s}^2
$$

## Final Result

- Mean Period: $T = 2.01 \pm 0.01\,\text{s}$
- Gravity: $g = (9.77 \pm 0.12)\,\text{m/s}^2$

## Interpretation

The calculated value of $g$ is close to the standard $9.81\,\text{m/s}^2$. The small discrepancy and uncertainty are typical for manual timing experiments where reaction time is the primary error source.