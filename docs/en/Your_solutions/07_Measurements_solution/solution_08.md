# Task 08 – Mass-Spring Measurements

## Problem Statement

Create a mass-spring simulator to measure the period of oscillation. Using $10$ trials for $10$ oscillations each, calculate the mean period, standard deviation, and the spring constant $k$ with its uncertainty.

## Theory

The period of a mass-spring system is:

$$
T = 2\pi \sqrt{\frac{m}{k}}
$$

Solving for $k$:

$$
k = \frac{4\pi^2 m}{T^2}
$$

The uncertainty in $k$ (assuming $m$ is exact) is:

$$
\Delta k = k \cdot \left( 2 \frac{\Delta T}{T} \right)
$$

## Step-by-Step Solution

### 1. Data Collection
(Simulated data for $10$ oscillations of a $0.5\,\text{kg}$ mass):
Times for $10T$: $14.2, 14.1, 14.3, 14.2, 14.0, 14.2, 14.4, 14.1, 14.2, 14.3$ (seconds).

### 2. Calculate Mean Period
Mean time for $10$ oscillations:

$$
\bar{t}_{10} = 14.2\,\text{s} \implies \bar{T} = 1.42\,\text{s}
$$

### 3. Standard Deviation
Using $\sigma_T \approx 0.011\,\text{s}$ (derived from sample variance).

### 4. Calculate $k$

$$
k = \frac{4\pi^2 (0.5)}{(1.42)^2} \approx \frac{19.739}{2.0164} \approx 9.79\,\text{N/m}
$$

### 5. Uncertainty in $k$

$$
\Delta k = 9.79 \cdot \left( 2 \cdot \frac{0.011}{1.42} \right) \approx 0.15\,\text{N/m}
$$

## Final Result

- Mean Period: $T = 1.42 \pm 0.01\,\text{s}$
- Spring Constant: $k = (9.79 \pm 0.15)\,\text{N/m}$

## Interpretation

The spring constant describes the stiffness of the spring. The calculated uncertainty accounts for the random fluctuations in timing measurements during the simulation.