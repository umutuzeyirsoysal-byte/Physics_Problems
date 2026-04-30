# Task 06 – Instrument Precision

## Problem Statement

A digital thermometer reads $25.4^\circ\text{C}$. Assuming the uncertainty is half the value of the last digit, calculate the absolute uncertainty of this measurement.

## Theory

For digital instruments, the "last digit" represents the resolution of the device. If the last digit is in the tenths place ($0.1$), then the smallest increment is $0.1$. The uncertainty $\Delta x$ is often taken as half of this smallest increment:

$$
\Delta x = \frac{\text{Resolution}}{2}
$$

## Step-by-Step Solution

1. **Determine resolution:**
   The reading is $25.4$. The last digit is in the $0.1$ position.
   Resolution $= 0.1^\circ\text{C}$.

2. **Apply the rule for uncertainty:**

$$
\Delta T = \frac{0.1^\circ\text{C}}{2} = 0.05^\circ\text{C}
$$

## Final Result

The absolute uncertainty is $0.05^\circ\text{C}$, and the measurement is recorded as $(25.40 \pm 0.05)^\circ\text{C}$.

## Interpretation

While the display only shows one decimal place, the uncertainty estimate suggests the true value lies between $25.35$ and $25.45$. This represents the limit of the instrument's precision.