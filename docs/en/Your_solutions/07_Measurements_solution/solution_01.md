# Task 01 – Propagation of Error I

## Problem Statement

The radius of a sphere is measured to be $r = (6.20 \pm 0.05)\text{ cm}$. Calculate the volume of the sphere and its associated absolute uncertainty.

## Theory

The volume $V$ of a sphere is given by:

$$
V = \frac{4}{3} \pi r^3
$$

When a quantity $y$ depends on a measured variable $x$ such that $y = f(x)$, the absolute uncertainty $\Delta y$ is calculated using the derivative:

$$
\Delta y = \left| \frac{df}{dx} \right| \Delta x
$$

For $V(r) = \frac{4}{3} \pi r^3$, the derivative is:

$$
\frac{dV}{dr} = 4 \pi r^2
$$

## Step-by-Step Solution

1. **Calculate the nominal volume:**

$$
V = \frac{4}{3} \pi (6.20)^3 \approx \frac{4}{3} \pi (238.328) \approx 998.306\,\text{cm}^3
$$

2. **Calculate the absolute uncertainty:**

$$
\Delta V = (4 \pi r^2) \Delta r
$$

$$
\Delta V = 4 \pi (6.20)^2 (0.05)
$$

$$
\Delta V = 4 \pi (38.44) (0.05) \approx 24.153\,\text{cm}^3
$$

3. **Round to significant figures:**
The uncertainty $0.05$ has one significant figure, but in measurements, we often keep two for intermediate steps or round the final uncertainty to the same decimal place as the value.

$$
V \approx 998\,\text{cm}^3, \quad \Delta V \approx 24\,\text{cm}^3
$$

## Final Result

The volume of the sphere is:

$$
V = (998 \pm 24)\,\text{cm}^3
$$

## Interpretation

The uncertainty in the radius is propagated and amplified because the radius is cubed in the volume formula. A small $0.8\%$ relative uncertainty in the radius results in a roughly $2.4\%$ relative uncertainty in the volume.