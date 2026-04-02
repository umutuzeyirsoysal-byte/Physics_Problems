# Task 04 – Energy & Momentum

## Problem Statement

A 0.5 kg block slides down a frictionless track from a height of 3.0 m. At the bottom, it collides and sticks to a 1.5 kg block initially at rest. Determine the speed of the combined mass just after the collision.

## Theory

This problem is solved in two phases:
1.  **Descent**: Conservation of mechanical energy applies as the first block slides down the frictionless track.
2.  **Collision**: Conservation of linear momentum applies during the perfectly inelastic collision.

Energy conservation equation:

$$
m_1 g h = \frac{1}{2} m_1 v_1^2
$$

Momentum conservation equation:

$$
m_1 v_1 + m_2 v_2 = (m_1 + m_2) v_f
$$

## Step-by-Step Solution

### Phase 1: Descent of the first block

Calculate the velocity $v_1$ of the first block at the bottom of the track:

$$
v_1 = \sqrt{2gh}
$$

Substitute the values ($h = 3.0\ \text{m}$, $g = 9.81\ \text{m/s}^2$):

$$
v_1 = \sqrt{2 \cdot 9.81 \cdot 3.0} = \sqrt{58.86} \approx 7.67\ \text{m/s}
$$

### Phase 2: Inelastic collision

Let $m_1 = 0.5\ \text{kg}$ and $m_2 = 1.5\ \text{kg}$. Since the second block is at rest, $v_2 = 0$.

$$
m_1 v_1 = (m_1 + m_2) v_f
$$

Solve for the final velocity $v_f$:

$$
v_f = \frac{m_1 v_1}{m_1 + m_2}
$$

Substitute the numerical values:

$$
v_f = \frac{0.5 \cdot 7.67}{0.5 + 1.5} = \frac{3.835}{2.0} \approx 1.92\ \text{m/s}
$$

## Final Result

The speed of the combined mass just after the collision is approximately $1.92\ \text{m/s}$.

## Interpretation

While total energy was conserved during the frictionless descent, kinetic energy is strongly dissipated during the inelastic collision. The quadrupling of the moving mass (from 0.5 kg to 2.0 kg) directly leads to the velocity being reduced to one-fourth of the pre-collision velocity.