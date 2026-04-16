# Task 04 – Force Comparison

## Problem Statement

Calculate the magnitude of the electric force and the gravitational force between an electron and a proton in a hydrogen atom ($r \approx 5.3 \times 10^{-11} \text{ m}$). What is the ratio $F_e/F_g$?

## Theory

The electric force is given by Coulomb's Law:

$$
F_e = k_e \frac{|q_1 q_2|}{r^2}
$$

The gravitational force is given by Newton's Law of Universal Gravitation:

$$
F_g = G \frac{m_1 m_2}{r^2}
$$

Constants:
* $k_e \approx 8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$
* $G \approx 6.67 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$
* $e \approx 1.6 \times 10^{-19} \text{ C}$
* $m_p \approx 1.67 \times 10^{-27} \text{ kg}$
* $m_e \approx 9.11 \times 10^{-31} \text{ kg}$

## Step-by-Step Solution

### 1. Calculate Electric Force

$$
F_e = \frac{(8.99 \times 10^9)(1.6 \times 10^{-19})^2}{(5.3 \times 10^{-11})^2} \approx 8.2 \times 10^{-8} \text{ N}
$$

### 2. Calculate Gravitational Force

$$
F_g = \frac{(6.67 \times 10^{-11})(1.67 \times 10^{-27})(9.11 \times 10^{-31})}{(5.3 \times 10^{-11})^2} \approx 3.6 \times 10^{-47} \text{ N}
$$

### 3. Calculate the Ratio

$$
\frac{F_e}{F_g} = \frac{k_e e^2}{G m_p m_e}
$$

Notice that $r^2$ cancels out, making the ratio independent of the distance:

$$
\frac{F_e}{F_g} \approx 2.27 \times 10^{39}
$$

## Final Result

* $F_e \approx 8.2 \times 10^{-8} \text{ N}$
* $F_g \approx 3.6 \times 10^{-47} \text{ N}$
* Ratio $F_e/F_g \approx 2.3 \times 10^{39}$

## Interpretation

The electric force is approximately 39 orders of magnitude stronger than the gravitational force. This confirms why gravity is negligible when dealing with atomic and subatomic interactions.