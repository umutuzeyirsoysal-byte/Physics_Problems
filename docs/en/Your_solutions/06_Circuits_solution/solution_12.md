# Task 12 – Transformer Currents

## Problem Statement

A transformer has $N_1 = 1000$ turns (primary) and $N_2 = 200$ turns (secondary).
- Primary voltage $V_1 = 120\,\text{V}$ (AC).
- Secondary current $I_2 = 3\,\text{A}$.
Calculate the secondary voltage $V_2$ and primary current $I_1$.

## Theory

For an ideal transformer, the ratio of voltages is equal to the ratio of turns:

$$
\frac{V_1}{V_2} = \frac{N_1}{N_2}
$$

Assuming $100\%$ efficiency, power is conserved ($P_1 = P_2$), leading to:

$$
\frac{I_1}{I_2} = \frac{N_2}{N_1}
$$

## Step-by-Step Solution

1. **Calculate Secondary Voltage:**

$$
V_2 = V_1 \left( \frac{N_2}{N_1} \right) = 120 \left( \frac{200}{1000} \right) = 120 \cdot 0.2 = 24\,\text{V}
$$

2. **Calculate Primary Current:**

$$
I_1 = I_2 \left( \frac{N_2}{N_1} \right) = 3 \left( \frac{200}{1000} \right) = 3 \cdot 0.2 = 0.6\,\text{A}
$$

## Final Result

- Secondary Voltage: $24\,\text{V}$
- Primary Current: $0.6\,\text{A}$

## Interpretation

This is a step-down transformer. As the voltage decreases by a factor of 5, the current on the primary side is 5 times smaller than the current on the secondary side.