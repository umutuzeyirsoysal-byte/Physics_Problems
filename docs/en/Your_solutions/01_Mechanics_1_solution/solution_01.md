# Task 01 – Projectile Motion

## Problem Statement

A projectile is fired from the ground with an initial velocity of $100 \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance.

* Derive the differential equations of motion in the horizontal and vertical directions.
* Determine the time of flight.
* Determine the maximum height.
* Determine the range.

## Theory

Projectile motion is a case of two-dimensional kinematics under constant acceleration. Neglecting air resistance, the only force acting on the object is gravity, which acts vertically downward.

Newton's Second Law states:

$$
\vec{F} = m\vec{a}
$$

In Cartesian coordinates, where $x$ is horizontal and $y$ is vertical (positive upwards), the acceleration components are:

$$
a_x = 0
$$

$$
a_y = -g
$$

## Step-by-Step Solution

### 1. Derivation of Equations of Motion

The acceleration is the second derivative of position with respect to time. For the horizontal direction:

$$
\frac{d^2x}{dt^2} = 0
$$

Integrating once with respect to time gives the velocity $v_x$:

$$
v_x(t) = v_{0x} = v_0 \cos(\theta)
$$

Integrating again gives the position $x(t)$:

$$
x(t) = v_0 \cos(\theta) t
$$

For the vertical direction:

$$
\frac{d^2y}{dt^2} = -g
$$

Integrating once gives the vertical velocity $v_y(t)$:

$$
v_y(t) = v_0 \sin(\theta) - gt
$$

Integrating again gives the position $y(t)$:

$$
y(t) = v_0 \sin(\theta) t - \frac{1}{2}gt^2
$$

### 2. Time of Flight ($T$)

The projectile returns to the ground when $y(T) = 0$. Using the position equation:

$$
v_0 \sin(\theta) T - \frac{1}{2}gT^2 = 0
$$

$$
T \left( v_0 \sin(\theta) - \frac{1}{2}gT \right) = 0
$$

Ignoring the trivial solution $T=0$:

$$
T = \frac{2v_0 \sin(\theta)}{g}
$$

Substituting $v_0 = 100 \text{ m/s}$, $\theta = 37^\circ$, and $g \approx 9.81 \text{ m/s}^2$:

$$
T = \frac{2(100) \sin(37^\circ)}{9.81} \approx 12.27 \text{ s}
$$

### 3. Maximum Height ($H$)

The maximum height is reached when the vertical velocity is zero ($v_y = 0$):

$$
0 = v_0 \sin(\theta) - gt_{up} \implies t_{up} = \frac{v_0 \sin(\theta)}{g}
$$

Substituting $t_{up}$ into the $y(t)$ equation:

$$
H = v_0 \sin(\theta) \left( \frac{v_0 \sin(\theta)}{g} \right) - \frac{1}{2}g \left( \frac{v_0 \sin(\theta)}{g} \right)^2
$$

$$
H = \frac{v_0^2 \sin^2(\theta)}{2g}
$$

Calculation:

$$
H = \frac{100^2 \sin^2(37^\circ)}{2(9.81)} \approx 184.62 \text{ m}
$$

### 4. Range ($R$)

The range is the horizontal distance traveled during the total time of flight $T$:

$$
R = x(T) = v_0 \cos(\theta) T
$$

$$
R = v_0 \cos(\theta) \left( \frac{2v_0 \sin(\theta)}{g} \right)
$$

Using the trigonometric identity $\sin(2\theta) = 2 \sin(\theta) \cos(\theta)$:

$$
R = \frac{v_0^2 \sin(2\theta)}{g}
$$

Calculation:

$$
R = \frac{100^2 \sin(74^\circ)}{9.81} \approx 979.88 \text{ m}
$$

## Final Result

* **Time of Flight:** $12.27 \text{ s}$
* **Maximum Height:** $184.62 \text{ m}$
* **Range:** $979.88 \text{ m}$

## Interpretation

The motion is parabolic. The horizontal velocity remains constant throughout the flight, while the vertical velocity changes linearly due to the constant acceleration of gravity. The time taken to reach the peak is exactly half of the total time of flight.