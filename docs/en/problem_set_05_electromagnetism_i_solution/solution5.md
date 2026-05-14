# Task 01 – Potential and energy

## Problem Statement

For a point charge $q = 4\ \mu\mathrm{C}$:
1. Calculate the potential at $r = 0.3\,\mathrm{m}$.
2. Calculate the potential difference between $0.3\,\mathrm{m}$ and $0.6\,\mathrm{m}$.
3. Calculate the work done to move a test charge $q_0 = 2\,\mu\mathrm{C}$ between these points.
4. Calculate the electric field intensity from the derivative of the potential.
5. Compare with Coulomb's law.

## Theory

The electric potential $V$ at a distance $r$ from a point charge $q$ is defined as the potential energy per unit charge:

$$
V(r) = \frac{1}{4\pi\epsilon_0} \frac{q}{r} = k \frac{q}{r}
$$

where $k \approx 8.99 \times 10^9\ \mathrm{N \cdot m^2 / C^2}$. The potential difference $\Delta V$ is:

$$
\Delta V = V(r_2) - V(r_1)
$$

The work $W$ required to move a charge $q_0$ through a potential difference is:

$$
W = q_0 \Delta V
$$

The relationship between the electric field $\vec{E}$ and the potential $V$ is given by the negative gradient:

$$
\vec{E} = -\nabla V
$$

## Step-by-Step Solution

**1. Potential at $r = 0.3\,\mathrm{m}$**

$$
V(0.3) = (8.99 \times 10^9) \frac{4 \times 10^{-6}}{0.3} \approx 1.199 \times 10^5\ \mathrm{V}
$$

**2. Potential difference**

First, calculate $V$ at $r = 0.6\,\mathrm{m}$:

$$
V(0.6) = (8.99 \times 10^9) \frac{4 \times 10^{-6}}{0.6} \approx 0.599 \times 10^5\ \mathrm{V}
$$

The potential difference $\Delta V = V(0.6) - V(0.3)$ is:

$$
\Delta V = 0.599 \times 10^5 - 1.199 \times 10^5 = -6.0 \times 10^4\ \mathrm{V}
$$

**3. Work done**

Moving $q_0 = 2\ \mu\mathrm{C}$ from $0.3\,\mathrm{m}$ to $0.6\,\mathrm{m}$:

$$
W = q_0 (V(0.6) - V(0.3)) = (2 \times 10^{-6})(-6.0 \times 10^4) = -0.12\ \mathrm{J}
$$

**4. Electric field from derivative**

In spherical coordinates, for a point charge:

$$
E_r = -\frac{dV}{dr} = -\frac{d}{dr} \left( \frac{kq}{r} \right) = -kq \left( -\frac{1}{r^2} \right) = \frac{kq}{r^2}
$$

**5. Comparison**

At $r = 0.3\,\mathrm{m}$:

$$
E = \frac{(8.99 \times 10^9)(4 \times 10^{-6})}{(0.3)^2} \approx 3.99 \times 10^5\ \mathrm{V/m}
$$

## Final Result

*   Potential at $0.3\,\mathrm{m}$: $1.2 \times 10^5\ \mathrm{V}$
*   Potential difference: $-6.0 \times 10^4\ \mathrm{V}$
*   Work: $-0.12\ \mathrm{J}$
*   Electric Field: $E(r) = \frac{kq}{r^2}$

## Interpretation

The negative work indicates that the field itself does work to push the positive test charge away from the source charge. The derivation of $E$ from $V$ confirms that the electric field is the spatial rate of change of the electric potential.
# Task 02 – Coulomb's force

## Problem Statement

Two point charges are given: $q_1 = 3\ \mu\mathrm{C}$ at $\vec{r}_1 = (0,0)$ and $q_2 = -5\ \mu\mathrm{C}$ at $\vec{r}_2 = (0.4, 0.3)\,\mathrm{m}$.
1. Determine the force vector acting on $q_2$.
2. Calculate its magnitude.
3. Determine the potential energy of the system.
4. Calculate the work required to separate the charges to a distance of $2\,\mathrm{m}$.

## Theory

Coulomb's Law in vector form for the force exerted by $q_1$ on $q_2$ is:

$$
\vec{F}_{12} = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{|\vec{r}_{12}|^3} \vec{r}_{12}
$$

where $\vec{r}_{12} = \vec{r}_2 - \vec{r}_1$. The potential energy $U$ of the system is:

$$
U = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r}
$$

## Step-by-Step Solution

**1. Force vector**

The displacement vector is $\vec{r}_{12} = (0.4 - 0, 0.3 - 0) = (0.4, 0.3)\,\mathrm{m}$.
The distance is $r = \sqrt{0.4^2 + 0.3^2} = 0.5\,\mathrm{m}$.

$$
\vec{F}_{2} = k \frac{q_1 q_2}{r^3} \vec{r}_{12} = (8.99 \times 10^9) \frac{(3 \times 10^{-6})(-5 \times 10^{-6})}{0.5^3} \begin{pmatrix} 0.4 \\ 0.3 \end{pmatrix}
$$

$$
\vec{F}_{2} = -1.0788 \begin{pmatrix} 0.4 \\ 0.3 \end{pmatrix} = \begin{pmatrix} -0.4315 \\ -0.3236 \end{pmatrix}\ \mathrm{N}
$$

**2. Magnitude**

$$
|\vec{F}_2| = \sqrt{(-0.4315)^2 + (-0.3236)^2} \approx 0.539\ \mathrm{N}
$$

**3. Potential energy**

$$
U_1 = k \frac{q_1 q_2}{r} = (8.99 \times 10^9) \frac{(3 \times 10^{-6})(-5 \times 10^{-6})}{0.5} = -0.2697\ \mathrm{J}
$$

**4. Work to separate**

The new energy at $r' = 2\,\mathrm{m}$ is:

$$
U_2 = (8.99 \times 10^9) \frac{-15 \times 10^{-12}}{2} = -0.0674\ \mathrm{J}
$$

The work $W_{ext}$ required is the change in potential energy:

$$
W = U_2 - U_1 = -0.0674 - (-0.2697) = 0.2023\ \mathrm{J}
$$

## Final Result

*   Force vector: $\vec{F}_2 \approx (-0.43, -0.32)\ \mathrm{N}$
*   Magnitude: $0.54\ \mathrm{N}$
*   Potential Energy: $-0.27\ \mathrm{J}$
*   Work: $0.20\ \mathrm{J}$

## Interpretation

The negative potential energy confirms an attractive system. Positive work is required to increase the separation, as we must overcome the attractive Coulomb force.
# Task 03 – Field at a point from a system of charges

## Problem Statement

Two point charges: $+q$ at $(-a, 0)$ and $+2q$ at $(a, 0)$.
1. Determine the field vector $\vec{E}$ at $(0, y)$, $(x, 0)$, and $(x, y)$.
2. Determine conditions for $E_x = 0$, $E_y = 0$, and $\vec{E} = 0$.
3. Calculate field for $a = 0.2\,\mathrm{m}$, $y = 0.3\,\mathrm{m}$, $q = 2\,\mu\mathrm{C}$ at $(0, y)$.
4. Investigate the limit $y \gg a$.
5. Does a point of zero field exist on the $y$-axis?

## Theory

The principle of superposition states that the total electric field is the vector sum of individual fields:

$$
\vec{E}_{total} = \sum \vec{E}_i = \sum k \frac{q_i}{r_i^2} \hat{r}_i
$$

## Step-by-Step Solution

**1. General Field $\vec{E}(x, y)$**

Let $\vec{r}_1 = (x+a, y)$ and $\vec{r}_2 = (x-a, y)$.

$$
\vec{E}(x, y) = \frac{kq}{((x+a)^2 + y^2)^{3/2}} \begin{pmatrix} x+a \\ y \end{pmatrix} + \frac{2kq}{((x-a)^2 + y^2)^{3/2}} \begin{pmatrix} x-a \\ y \end{pmatrix}
$$

For $(0, y)$:

$$
\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} \begin{pmatrix} a \\ y \end{pmatrix} + \frac{2kq}{(a^2 + y^2)^{3/2}} \begin{pmatrix} -a \\ y \end{pmatrix} = \frac{kq}{(a^2 + y^2)^{3/2}} \begin{pmatrix} -a \\ 3y \end{pmatrix}
$$

**2. Zero Field Conditions**

For $E_y = 0$ on the x-axis ($y=0$): This is always true for points on the x-axis excluding the charges.
For $E_x = 0$ on the x-axis:

$$
\frac{q}{(x+a)^2} = \frac{2q}{(a-x)^2} \implies (a-x)^2 = 2(x+a)^2
$$

Solving for $x$ between $-a$ and $a$: $x = a(1 - 2\sqrt{2})/(1 + \sqrt{2})$. Since $2q > q$, the equilibrium point is closer to the smaller charge.

**3. Numerical Calculation at $(0, 0.3)$**

$r = \sqrt{0.2^2 + 0.3^2} \approx 0.3606$.

$$
E_x = \frac{k q (-a)}{r^3} \approx -1.54 \times 10^4\ \mathrm{V/m}, \quad E_y = \frac{3 k q y}{r^3} \approx 1.38 \times 10^5\ \mathrm{V/m}
$$

**4. Limit $y \gg a$**

As $y \to \infty$, $r \approx y$:

$$
\vec{E} \approx \frac{kq}{y^3} \begin{pmatrix} -a \\ 3y \end{pmatrix} \approx \begin{pmatrix} 0 \\ \frac{3kq}{y^2} \end{pmatrix}
$$

This matches the field of a single charge $3q$ at the origin.

## Final Result

The field at $(0, y)$ is $\vec{E} = \frac{kq}{(a^2+y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$.

## Interpretation

At large distances, the system behaves as a single point charge of value $q_{total} = 3q$. The zero field point exists only on the axis connecting the charges (x-axis), not the y-axis, because $E_y$ components from both positive charges always point in the same direction for $y \neq 0$.
# Task 04 – Motion of a particle in a uniform field

## Problem Statement

Given: $m = 0.02\ \mathrm{kg}$, $q = 1\ \mathrm{mC}$, $\vec{E} = (30, 100)\,\mathrm{N/C}$, $\vec{v}(0) = (20, 0)\,\mathrm{m/s}$, $\vec{r}(0) = (0, 0)$.
1. Solve equations of motion.
2. Trajectory.
3. Time to reach $v_y = 50\,\mathrm{m/s}$.
4. Kinetic energy at $t = 0.05\,\mathrm{s}$.
5. Energy balance check.

## Theory

From Newton's second law:

$$
\vec{F} = q\vec{E} = m\vec{a} \implies \vec{a} = \frac{q}{m}\vec{E}
$$

Since $\vec{E}$ is constant, $\vec{a}$ is constant.

## Step-by-Step Solution

**1. Equations of Motion**

$$
a_x = \frac{10^{-3} \cdot 30}{0.02} = 1.5\ \mathrm{m/s^2}, \quad a_y = \frac{10^{-3} \cdot 100}{0.02} = 5.0\ \mathrm{m/s^2}
$$

Integration:

$$
v_x(t) = 20 + 1.5t, \quad v_y(t) = 5t
$$

$$
x(t) = 20t + 0.75t^2, \quad y(t) = 2.5t^2
$$

**2. Trajectory**

Since $t = \sqrt{y/2.5}$, the trajectory $x(y)$ is a parabola:

$$
x = 20\sqrt{\frac{y}{2.5}} + 0.75\left(\frac{y}{2.5}\right)
$$

**3. Time for $v_y = 50$**

$$
50 = 5t \implies t = 10\ \mathrm{s}
$$

**4. Kinetic Energy at $t = 0.05$**

$v_x = 20 + 1.5(0.05) = 20.075$, $v_y = 5(0.05) = 0.25$.

$$
E_k = \frac{1}{2}m(v_x^2 + v_y^2) = 0.01(20.075^2 + 0.25^2) \approx 4.0307\ \mathrm{J}
$$

**5. Energy Balance**

Work done by field $W = q\vec{E} \cdot \Delta\vec{r}$. At $t=0.05$: $x \approx 1.0018$, $y \approx 0.00625$.

$$
W = 10^{-3}(30 \cdot 1.0018 + 100 \cdot 0.00625) \approx 0.0307\ \mathrm{J}
$$

Initial $E_k = 0.5(0.02)(20^2) = 4\ \mathrm{J}$. Total $E = 4 + 0.0307 = 4.0307\ \mathrm{J}$. Consistent.

## Final Result

The particle follows a parabolic path. $E_k(0.05\mathrm{s}) = 4.031\ \mathrm{J}$.

## Interpretation

The motion is analogous to projectile motion in a gravitational field, but with an acceleration component in both dimensions due to the orientation of the $\vec{E}$ field.
# Task 04 – Motion of a particle in a uniform field

## Problem Statement

Given: $m = 0.02\ \mathrm{kg}$, $q = 1\ \mathrm{mC}$, $\vec{E} = (30, 100)\,\mathrm{N/C}$, $\vec{v}(0) = (20, 0)\,\mathrm{m/s}$, $\vec{r}(0) = (0, 0)$.
1. Solve equations of motion.
2. Trajectory.
3. Time to reach $v_y = 50\,\mathrm{m/s}$.
4. Kinetic energy at $t = 0.05\,\mathrm{s}$.
5. Energy balance check.

## Theory

From Newton's second law:

$$
\vec{F} = q\vec{E} = m\vec{a} \implies \vec{a} = \frac{q}{m}\vec{E}
$$

Since $\vec{E}$ is constant, $\vec{a}$ is constant.

## Step-by-Step Solution

**1. Equations of Motion**

$$
a_x = \frac{10^{-3} \cdot 30}{0.02} = 1.5\ \mathrm{m/s^2}, \quad a_y = \frac{10^{-3} \cdot 100}{0.02} = 5.0\ \mathrm{m/s^2}
$$

Integration:

$$
v_x(t) = 20 + 1.5t, \quad v_y(t) = 5t
$$

$$
x(t) = 20t + 0.75t^2, \quad y(t) = 2.5t^2
$$

**2. Trajectory**

Since $t = \sqrt{y/2.5}$, the trajectory $x(y)$ is a parabola:

$$
x = 20\sqrt{\frac{y}{2.5}} + 0.75\left(\frac{y}{2.5}\right)
$$

**3. Time for $v_y = 50$**

$$
50 = 5t \implies t = 10\ \mathrm{s}
$$

**4. Kinetic Energy at $t = 0.05$**

$v_x = 20 + 1.5(0.05) = 20.075$, $v_y = 5(0.05) = 0.25$.

$$
E_k = \frac{1}{2}m(v_x^2 + v_y^2) = 0.01(20.075^2 + 0.25^2) \approx 4.0307\ \mathrm{J}
$$

**5. Energy Balance**

Work done by field $W = q\vec{E} \cdot \Delta\vec{r}$. At $t=0.05$: $x \approx 1.0018$, $y \approx 0.00625$.

$$
W = 10^{-3}(30 \cdot 1.0018 + 100 \cdot 0.00625) \approx 0.0307\ \mathrm{J}
$$

Initial $E_k = 0.5(0.02)(20^2) = 4\ \mathrm{J}$. Total $E = 4 + 0.0307 = 4.0307\ \mathrm{J}$. Consistent.

## Final Result

The particle follows a parabolic path. $E_k(0.05\mathrm{s}) = 4.031\ \mathrm{J}$.

## Interpretation

The motion is analogous to projectile motion in a gravitational field, but with an acceleration component in both dimensions due to the orientation of the $\vec{E}$ field.
# Task 06 – 2D field map

## Problem Statement

System: any three charges in a plane.
1. Implement a function calculating the field vector $\vec{E}(x, y)$.
2. Generate a vector field map.
3. Find the equilibrium point numerically.
4. Investigate the stability of the equilibrium point.
5. Compare with the case of two charges.

## Theory

The electric field $\vec{E}$ at position $\vec{r}$ due to $N$ point charges is the sum of individual fields:

$$
\vec{E}(\vec{r}) = \sum_{i=1}^{N} \frac{k q_i}{|\vec{r} - \vec{r}_i|^3} (\vec{r} - \vec{r}_i)
$$

An equilibrium point exists where $\vec{E}(\vec{r}) = 0$. Stability is determined by the potential $V$. According to Earnshaw's Theorem, a point charge cannot be in stable stationary equilibrium under the influence of electrostatic forces alone.

## Step-by-Step Solution

**1. Function Implementation**

For three charges $q_1, q_2, q_3$ at $\vec{r}_1, \vec{r}_2, \vec{r}_3$:

$$
\vec{E}(x, y) = \begin{pmatrix} E_x \\ E_y \end{pmatrix} = \sum_{i=1}^{3} \frac{k q_i}{((x-x_i)^2 + (y-y_i)^2)^{3/2}} \begin{pmatrix} x-x_i \\ y-y_i \end{pmatrix}
$$

**2. Numerical Equilibrium Search**

Equilibrium points are found by solving the non-linear system $E_x(x, y) = 0$ and $E_y(x, y) = 0$ using iterative methods like Newton-Raphson.

**3. Stability Analysis**

To check stability, we evaluate the Hessian matrix of the potential $V$:

$$
H = \begin{pmatrix} 
\frac{\partial^2 V}{\partial x^2} & \frac{\partial^2 V}{\partial x \partial y} \\ 
\frac{\partial^2 V}{\partial y \partial x} & \frac{\partial^2 V}{\partial y^2} 
\end{pmatrix}
$$

Since $\nabla^2 V = 0$ (Laplace equation) in charge-free regions, the eigenvalues of $H$ must have opposite signs (saddle point), confirming instability.

## Final Result

The system requires an HTML/JavaScript implementation to visualize the vector field using a grid of arrows and a root-finding algorithm to mark $\vec{E}=0$.

## Interpretation

In a 2D plane, equilibrium points for like charges typically appear in the central region. These points are always saddle points; a particle might be stable against displacements in one direction but will be accelerated away in another.
# Task 07 – Motion in a central field

## Problem Statement

For field $E(r) = k \frac{Q}{r^2} \hat{r}$:
1. Write the equation of motion.
2. Consider radial motion.
3. Implement the RK4 method.
4. Investigate positive and negative energy.
5. Compare with gravitational analogy.

## Theory

The force on a particle of charge $q$ and mass $m$ is $\vec{F} = q\vec{E}$. The equation of motion is:

$$
m \frac{d^2\vec{r}}{dt^2} = \frac{kQq}{r^3} \vec{r}
$$

## Step-by-Step Solution

**1. Equation of Motion**

Dividing by $m$ and using $C = \frac{kQq}{m}$:

$$
\ddot{\vec{r}} = \frac{C}{r^3} \vec{r}
$$

**2. Radial Motion**

If the motion is purely radial (angular momentum $L=0$):

$$
\ddot{r} = \frac{C}{r^2}
$$

**3. RK4 Implementation**

We transform the second-order ODE into a system of first-order ODEs:

$$
\begin{align}
\frac{d\vec{r}}{dt} &= \vec{v} \\
\frac{d\vec{v}}{dt} &= \frac{C}{|\vec{r}|^3} \vec{r}
\end{align}
$$

The Runge-Kutta 4th order method updates the state $(\vec{r}_n, \vec{v}_n)$ by calculating four weighted slopes ($k_1$ through $k_4$) per step.

**4. Energy States**

Total Energy $E = \frac{1}{2}mv^2 + \frac{kQq}{r}$.
*   $E < 0$: Bound orbits (ellipses), only possible if $Qq < 0$ (attractive).
*   $E > 0$: Unbound orbits (hyperbolas).
*   $E = 0$: Parabolic trajectory.

## Final Result

Numerical simulation shows that for attractive charges ($Qq < 0$), the particle follows Keplerian orbits. For repulsive charges, the particle is deflected in a scattering trajectory.

## Interpretation

The $1/r^2$ dependence makes this mathematically identical to the gravitational problem. The key difference is that $C$ can be positive (repulsion), which does not exist in standard Newtonian gravity.
# Task 08 – Energy of a three-charge system

## Problem Statement

1. Write the total energy of the system.
2. Calculate energy for an equilateral triangle configuration.
3. Investigate sign changes.
4. Find minimum energy configuration.
5. Interpret stability.

## Theory

The total electrostatic potential energy $U$ of a system of $N$ point charges is the sum over all distinct pairs:

$$
U = \sum_{i=1}^{N} \sum_{j>i}^{N} \frac{k q_i q_j}{r_{ij}}
$$

## Step-by-Step Solution

**1. Total Energy Expression**

For three charges $q_1, q_2, q_3$:

$$
U = k \left( \frac{q_1 q_2}{r_{12}} + \frac{q_1 q_3}{r_{13}} + \frac{q_2 q_3}{r_{23}} \right)
$$

**2. Equilateral Triangle**

Let all sides be $L$ and all charges be $q$:

$$
U = k \left( \frac{q^2}{L} + \frac{q^2}{L} + \frac{q^2}{L} \right) = \frac{3kq^2}{L}
$$

**3. Changing Sign**

If $q_3 \to -q$:

$$
U = k \left( \frac{q^2}{L} - \frac{q^2}{L} - \frac{q^2}{L} \right) = -\frac{kq^2}{L}
$$

**4. Minimum Energy Configuration**

If charges are free to move, like charges will maximize $r_{ij}$ (move to infinity), leading to $U \to 0$. For opposite charges, the minimum energy is $U \to -\infty$ as $r \to 0$ (point charges collapsing).

## Final Result

Energy is a scalar quantity. For like charges, $U > 0$; for systems with mixed signs, $U$ can be negative.

## Interpretation

The system is not self-stable. Like charges repel to infinity to minimize $U$. Opposite charges attract and "collapse" unless prevented by other forces (like quantum effects or mechanical constraints).
# Task 09 – Dipole in an external field

## Problem Statement

1. Derive torque formula.
2. Calculate potential energy.
3. Determine equation of angular motion.
4. Linearize for small displacements.
5. Interpret as harmonic oscillator.

## Theory

A dipole consists of two charges $+q$ and $-q$ separated by $\vec{d}$. The dipole moment is $\vec{p} = q\vec{d}$.

## Step-by-Step Solution

**1. Torque ($\vec{\tau}$)**

The forces are $\vec{F}_+ = q\vec{E}$ and $\vec{F}_- = -q\vec{E}$.

$$
\vec{\tau} = \vec{r}_+ \times \vec{F}_+ + \vec{r}_- \times \vec{F}_- = \vec{d} \times (q\vec{E}) = \vec{p} \times \vec{E}
$$

Magnitude: $\tau = -pE \sin \theta$ (restoring torque).

**2. Potential Energy ($U$)**

$$
U = -\int \tau d\theta = -\int pE \sin \theta d\theta = -pE \cos \theta = -\vec{p} \cdot \vec{E}
$$

**3. Angular Motion**

Using $I \ddot{\theta} = \tau$, where $I$ is the moment of inertia:

$$
I \frac{d^2\theta}{dt^2} + pE \sin \theta = 0
$$

**4. Linearization**

For small $\theta$, $\sin \theta \approx \theta$:

$$
I \ddot{\theta} + pE \theta = 0 \implies \ddot{\theta} + \left( \frac{pE}{I} \right) \theta = 0
$$

## Final Result

The equation takes the form $\ddot{\theta} + \omega^2 \theta = 0$ with:

$$
\omega = \sqrt{\frac{pE}{I}}
$$

## Interpretation

A dipole in a uniform field performs Simple Harmonic Motion (SHM) around the field direction. The field acts as a "torsional spring" trying to align the dipole moment with the field lines.
# Task 10 – Field flux (Gauss's Law)

## Problem Statement

1. Define electric field flux.
2. Consider a sphere around a point charge.
3. Implement discrete approximation.
4. Investigate grid dependence.
5. Compare with analytical results.

## Theory

Electric flux $\Phi_E$ through a surface $S$ is:

$$
\Phi_E = \oint_S \vec{E} \cdot d\vec{A}
$$

Gauss's Law states $\Phi_E = Q_{encl} / \epsilon_0$.

## Step-by-Step Solution

**1. Analytical Case**

For a sphere of radius $R$ centered on charge $q$:

$$
\Phi_E = \oint \frac{kq}{R^2} \hat{r} \cdot (R^2 \sin \theta d\theta d\phi \hat{r}) = kq \int_0^\pi \sin \theta d\theta \int_0^{2\pi} d\phi = 4\pi kq = \frac{q}{\epsilon_0}
$$

**2. Discrete Approximation**

We divide the sphere into $N$ small area elements $\Delta A_i$.

$$
\Phi_{approx} = \sum_{i=1}^{N} \vec{E}(\vec{r}_i) \cdot \vec{n}_i \Delta A_i
$$

Using spherical coordinates, $\Delta A \approx R^2 \sin \theta \Delta \theta \Delta \phi$.

**3. Grid Dependence**

As the number of grid points ($N_\theta, N_\phi$) increases, the sum $\sum \sin \theta \Delta \theta \Delta \phi$ converges to the integral value $4\pi$. The error scales as $1/N$.

## Final Result

The discrete flux calculation converges to $q/\epsilon_0$ regardless of the radius $R$, verifying that flux is independent of the surface size as long as the charge is enclosed.

## Interpretation

Numerical verification of Gauss's Law demonstrates the inverse-square nature of the field. The $1/r^2$ fall-off of the field strength is perfectly cancelled by the $r^2$ growth of the surface area.