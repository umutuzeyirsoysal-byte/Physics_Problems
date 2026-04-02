# Task 07 – Dynamics with Friction

## Problem Statement

A 5 kg block is placed on a 10 kg block. A horizontal force of 45 N is applied to the 10 kg block, and the 5 kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is 0.2. Find the acceleration of the 10 kg block.

## Theory

Newton's Second Law describes the motion of a body under net force:

$$
\Sigma F = m a
$$

The magnitude of the kinetic friction force is proportional to the normal force:

$$
F_k = \mu_k N
$$

Because the 5 kg block is tied to the wall, it remains stationary relative to the ground. The 10 kg block slides underneath it. This creates two distinct surfaces of kinetic friction opposing the motion of the 10 kg block:
1. Between the 5 kg block and the 10 kg block.
2. Between the 10 kg block and the floor.

## Step-by-Step Solution

Let $m_1 = 5\ \text{kg}$ (top block) and $m_2 = 10\ \text{kg}$ (bottom block). The applied force is $F_{\text{app}} = 45\ \text{N}$. The kinetic friction coefficient is $\mu_k = 0.2$. Let $g = 9.81\ \text{m/s}^2$.

### Normal Forces

The normal force between the top block and the bottom block is:

$$
N_1 = m_1 g
$$

The normal force between the bottom block and the ground must support the weight of both blocks:

$$
N_2 = (m_1 + m_2) g
$$

### Friction Forces

The friction force $f_1$ exerted by the 5 kg block on the 10 kg block:

$$
\begin{align}
f_1 &= \mu_k N_1 \\
    &= \mu_k m_1 g \\
    &= 0.2 \cdot 5 \cdot 9.81 \\
    &= 9.81\ \text{N}
\end{align}
$$

The friction force $f_2$ exerted by the floor on the 10 kg block:

$$
\begin{align}
f_2 &= \mu_k N_2 \\
    &= \mu_k (m_1 + m_2) g \\
    &= 0.2 \cdot 15 \cdot 9.81 \\
    &= 29.43\ \text{N}
\end{align}
$$

### Equation of Motion for the 10 kg Block

The net horizontal force acting on the bottom block is the applied force minus both frictional forces:

$$
F_{\text{net}} = F_{\text{app}} - f_1 - f_2
$$

Substitute the net force into Newton's Second Law to find the acceleration $a$:

$$
m_2 a = F_{\text{app}} - f_1 - f_2
$$

$$
10 a = 45 - 9.81 - 29.43
$$

$$
10 a = 5.76
$$

$$
a = 0.576\ \text{m/s}^2
$$

## Final Result

The acceleration of the 10 kg block is $0.576\ \text{m/s}^2$.

## Interpretation

Both interfaces contribute significantly to the total resistive force. The upper friction acts as a drag on the moving block, while the lower friction acts normally against the ground. The applied force (45 N) is just slightly larger than the total required to overcome these two friction sources (39.24 N), resulting in a small positive acceleration.