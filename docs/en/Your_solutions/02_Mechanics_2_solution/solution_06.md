# Task 06 – Energy Dissipation

## Problem Statement

A tennis ball is dropped from a height of $2.0\ \text{m}$. After each bounce, it loses 30% of its mechanical energy. Calculate the height to which it rises after the second bounce.

## Theory

The mechanical energy of the ball at maximum height is purely gravitational potential energy:

$$
E = mgh
$$

If the ball loses 30% of its energy upon bouncing, it retains 70% of its previous energy. The energy after the $n$-th bounce is:

$$
E_n = 0.70 \cdot E_{n-1}
$$

Because mass $m$ and gravity $g$ remain constant, the maximum height reached is directly proportional to the retained mechanical energy.

## Step-by-Step Solution

Let $h_0 = 2.0\ \text{m}$ be the initial height.

After the first bounce, the retained energy is $E_1 = 0.70 E_0$. The corresponding height $h_1$ is:

$$
\begin{align}
m g h_1 &= 0.70 m g h_0 \\
h_1 &= 0.70 h_0
\end{align}
$$

After the second bounce, the retained energy is $E_2 = 0.70 E_1$. The height $h_2$ is:

$$
\begin{align}
m g h_2 &= 0.70 m g h_1 \\
h_2 &= 0.70 (0.70 h_0) \\
h_2 &= 0.49 h_0
\end{align}
$$

Substitute the initial height:

$$
h_2 = 0.49 \cdot 2.0\ \text{m} = 0.98\ \text{m}
$$

## Final Result

The tennis ball rises to a height of $0.98\ \text{m}$ after the second bounce.

## Interpretation

The geometric progression of energy loss leads to an exponential decay in the maximum rebound height. After merely two bounces, the ball retains less than half ($49\%$) of its original mechanical energy.