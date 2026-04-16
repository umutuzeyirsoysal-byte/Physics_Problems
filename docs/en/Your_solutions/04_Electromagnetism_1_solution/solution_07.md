# Task 07 – Cyclotron Motion

## Problem Statement

An electron is accelerated from rest through a potential difference of $5000\text{ V}$. It then enters a region of uniform magnetic field $B = 0.1\text{ T}$, perpendicular to its velocity. What is the radius of the circular path it will follow?

## Theory

When a charge $q$ is accelerated through a potential difference $V$, the work done by the electric field is converted into kinetic energy:

$$
qV = \frac{1}{2} m v^2
$$

Once the electron enters the uniform magnetic field $\vec{B}$, it experiences a magnetic force $\vec{F}_m = q(\vec{v} \times \vec{B})$. Since the velocity is perpendicular to the field, the magnitude is $F_m = qvB$. This force acts as a centripetal force, keeping the particle in a circular orbit:

$$
qvB = \frac{mv^2}{R}
$$



## Step-by-Step Solution

### 1. Find the Velocity ($v$)
We first determine the speed of the electron after acceleration:

$$
v = \sqrt{\frac{2qV}{m}}
$$

Using the following constants:
* $q = e \approx 1.602 \times 10^{-19}\text{ C}$
* $m = m_e \approx 9.109 \times 10^{-31}\text{ kg}$
* $V = 5000\text{ V}$

$$
v = \sqrt{\frac{2(1.602 \times 10^{-19})(5000)}{9.109 \times 10^{-31}}} \approx 4.19 \times 10^7\text{ m/s}
$$

### 2. Derive the Radius Formula
From the centripetal force balance, we solve for $R$:

$$
R = \frac{mv}{qB}
$$

### 3. Calculate the Final Value
Substitute the velocity $v$, the magnetic field $B = 0.1\text{ T}$, and the particle constants:

$$
R = \frac{(9.109 \times 10^{-31})(4.19 \times 10^7)}{(1.602 \times 10^{-19})(0.1)}
$$

$$
R = \frac{3.817 \times 10^{-23}}{1.602 \times 10^{-20}}
$$

$$
R \approx 0.00238\text{ m}
$$

## Final Result

The radius of the circular path is:

$$
R \approx 2.38\text{ mm}
$$

## Interpretation

The radius of the path (often called the Larmor radius or gyroradius) is proportional to the momentum of the particle and inversely proportional to the charge and field strength. Because electrons have a very small mass-to-charge ratio, they exhibit very tight curvatures even at high velocities.