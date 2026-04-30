# Task 02 – Propagation of Error II

## Problem Statement

The length and width of a rectangular plate are $L = (15.3 \pm 0.1)\text{ cm}$ and $W = (8.4 \pm 0.1)\text{ cm}$. Calculate the area and its uncertainty.

## Theory

The area $A$ is:

$$
A = L \cdot W
$$

For a product $y = x_1 x_2$, the relative uncertainty adds in quadrature:

$$
\frac{\Delta A}{A} = \sqrt{\left( \frac{\Delta L}{L} \right)^2 + \left( \frac{\Delta W}{W} \right)^2}
$$

## Step-by-Step Solution

1. **Nominal Area:**

$$
A = 15.3 \cdot 8.4 = 128.52\,\text{cm}^2
$$

2. **Relative Uncertainties:**

$$
\frac{\Delta L}{L} = \frac{0.1}{15.3} \approx 0.006536
$$

$$
\frac{\Delta W}{W} = \frac{0.1}{8.4} \approx 0.011905
$$

3. **Total Relative Uncertainty:**

$$
\frac{\Delta A}{A} = \sqrt{(0.006536)^2 + (0.011905)^2} \approx \sqrt{0.0000427 + 0.0001417} \approx 0.01358
$$

4. **Absolute Uncertainty:**

$$
\Delta A = A \cdot 0.01358 = 128.52 \cdot 0.01358 \approx 1.745\,\text{cm}^2
$$

## Final Result

Rounding to appropriate precision:

$$
A = (128.5 \pm 1.7)\,\text{cm}^2
$$

## Interpretation

The uncertainty in the width contributes more to the total error than the length because the width is smaller, making its relative error larger.