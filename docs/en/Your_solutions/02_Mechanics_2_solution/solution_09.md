# Task 09 – Vertical Throw with Drag

## Problem Statement

Given the equation of motion for a mass under gravity with linear air resistance $m\frac{dv}{dt} = -mg - kv$ with initial conditions $v(0)=v_0$, $x(0)=10$:
* Solve the equation by analytical methods.
* Determine the maximum height.
* Compare with the case without drag.
* Perform a numerical simulation using Python.

## Theory

The given first-order linear ordinary differential equation can be solved by separating variables. The kinematic relationship $\frac{dx}{dt} = v$ allows finding the position. 

## Step-by-Step Solution

### Analytical Solution for Velocity

Divide by $m$ to separate variables:

$$
\frac{dv}{dt} = -g - \frac{k}{m}v
$$

$$
\frac{dv}{dt} = -\frac{k}{m} \left( \frac{mg}{k} + v \right)
$$

Rearrange to integrate:

$$
\int_{v_0}^{v(t)} \frac{dv}{v + \frac{mg}{k}} = \int_{0}^{t} -\frac{k}{m} dt
$$

$$
\left[ \ln \left| v + \frac{mg}{k} \right| \right]_{v_0}^{v(t)} = -\frac{k}{m} t
$$

$$
\ln \left( \frac{v(t) + \frac{mg}{k}}{v_0 + \frac{mg}{k}} \right) = -\frac{k}{m} t
$$

Take the exponential of both sides:

$$
v(t) + \frac{mg}{k} = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t}
$$

$$
v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t} - \frac{mg}{k}
$$

### Maximum Height

The maximum height is reached when velocity is zero, $v(t_{max}) = 0$:

$$
0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t_{max}} - \frac{mg}{k}
$$

$$
e^{\frac{k}{m} t_{max}} = \frac{v_0 + \frac{mg}{k}}{\frac{mg}{k}} = 1 + \frac{k v_0}{mg}
$$

$$
t_{max} = \frac{m}{k} \ln \left( 1 + \frac{k v_0}{mg} \right)
$$

To find $x(t)$, integrate $v(t)$:

$$
\begin{align}
x(t) &= \int v(t) dt \\
     &= \int \left[ \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t} - \frac{mg}{k} \right] dt \\
     &= -\frac{m}{k} \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t} - \frac{mg}{k} t + C
\end{align}
$$

Using $x(0) = 10$:

$$
10 = -\frac{m}{k} \left( v_0 + \frac{mg}{k} \right) + C
$$

$$
C = 10 + \frac{m}{k} \left( v_0 + \frac{mg}{k} \right)
$$

Substitute $t_{max}$ into $x(t)$ to get $x_{max}$:

$$
x_{max} = 10 + \frac{m}{k} v_0 - \frac{m^2 g}{k^2} \ln \left( 1 + \frac{k v_0}{mg} \right)
$$

### Comparison with No Drag

Without drag ($k = 0$), mechanical energy is conserved:

$$
\Delta h_{no\_drag} = \frac{v_0^2}{2g}
$$

With drag, continuous mechanical energy dissipation occurs, meaning the kinetic energy is converted into heat due to air friction. Consequently, $x_{max} < 10 + \frac{v_0^2}{2g}$.

### Python Numerical Simulation

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp

# Parameters
m = 1.0     # kg
g = 9.81    # m/s^2
k = 0.5     # kg/s (drag coefficient)
v0 = 20.0   # m/s
x0 = 10.0   # m

def equations(t, y):
    x, v = y
    dxdt = v
    dvdt = -g - (k/m) * v
    return [dxdt, dvdt]

# Event function to stop when object hits the ground (x=0)
def hit_ground(t, y): return y[0]
hit_ground.terminal = True
hit_ground.direction = -1

t_span = (0, 10)
y0 = [x0, v0]

solution = solve_ivp(equations, t_span, y0, events=hit_ground, dense_output=True)

t = np.linspace(0, solution.t[-1], 200)
x, v = solution.sol(t)

plt.plot(t, x, label='Position $x(t)$')
plt.xlabel('Time (s)')
plt.ylabel('Height (m)')
plt.title('Vertical Throw with Linear Drag')
plt.grid()
plt.legend()
plt.show()