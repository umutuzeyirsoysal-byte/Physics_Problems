# Task 14 – RLC Circuit

## Problem Statement

Write the differential equation for a series RLC circuit and compare it to the damped harmonic oscillator.

## Theory

A series RLC circuit consists of a resistor $R$, inductor $L$, and capacitor $C$ in series with a voltage source $V(t)$. The sum of voltages is:

$$
V_L + V_R + V_C = V(t)
$$

## Step-by-Step Solution

### 1. Circuit Equation
Using $V_L = L \frac{dI}{dt}$, $V_R = IR$, and $V_C = \frac{q}{C}$, where $I = \frac{dq}{dt}$:

$$
L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{1}{C} q = V(t)
$$

### 2. Damped Harmonic Oscillator Equation
The equation for a mass $m$ on a spring with constant $k$ and damping $b$ is:

$$
m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F(t)
$$

### 3. Comparison Table

| Mechanical System | Electrical System |
| :--- | :--- |
| Displacement ($x$) | Charge ($q$) |
| Velocity ($v$) | Current ($I$) |
| Mass ($m$) | Inductance ($L$) |
| Damping ($b$) | Resistance ($R$) |
| Spring Constant ($k$) | Reciprocal Capacitance ($1/C$) |
| External Force ($F$) | Electromotive Force ($V$) |

## Final Result

The RLC circuit is mathematically identical to a damped harmonic oscillator, with the differential equation:

$$
L \ddot{q} + R \dot{q} + \frac{1}{C} q = V(t)
$$

## Interpretation

The inductor provides "inertia" (storing energy in a magnetic field), the resistor provides "friction" (dissipating energy as heat), and the capacitor provides "restoring force" (storing energy in an electric field).