# Task 01 – Newton's second law (constant force)

## Problem Statement

A constant force acts on a body of mass $m = 2\ \mathrm{kg}$:

$$
\vec{F} =
\begin{pmatrix}
6 \\
2
\end{pmatrix}
\ \mathrm{N}
$$

The body starts with an initial velocity $\vec{v}(0)$ from the initial position $\vec{r}(0)$:

$$
\vec{v}(0) =
\begin{pmatrix}
1 \\
-1
\end{pmatrix}
\ \mathrm{\frac{m}{s}}
$$

$$
\vec{r}(0) =
\begin{pmatrix}
0 \\
0
\end{pmatrix}
\ \mathrm{m}
$$

Determine the acceleration $\vec{a}(t)$, velocity $\vec{v}(t)$, and position $\vec{r}(t)$. Draw the trajectory of the motion. Calculate the work done by the force at time $t=3\ \mathrm{s}$ and check the consistency with the work-energy theorem.

## Theory

Newton's second law relates the net force acting on an object to its acceleration:

$$
\vec{F} = m\vec{a}
$$

For a constant force, the acceleration is constant. Kinematic quantities are obtained by successive time integration of the acceleration:

$$
\vec{v}(t) = \int \vec{a} \, dt
$$

$$
\vec{r}(t) = \int \vec{v}(t) \, dt
$$

The work done by a constant force along a displacement $\Delta\vec{r}$ is the dot product:

$$
W = \vec{F} \cdot \Delta\vec{r}
$$

The work-energy theorem states that the net work done on a body equals its change in kinetic energy $T$:

$$
W = \Delta T = T_f - T_i
$$

## Step-by-Step Solution

The acceleration vector is determined by dividing the force vector by the mass:

$$
\vec{a}(t) = \frac{1}{m}\vec{F} = \frac{1}{2}
\begin{pmatrix}
6 \\
2
\end{pmatrix}
=
\begin{pmatrix}
3 \\
1
\end{pmatrix}
\ \mathrm{\frac{m}{s^2}}
$$

The velocity vector is found by integrating the constant acceleration and adding the initial velocity:

$$
\vec{v}(t) = \vec{v}(0) + \vec{a}t
$$

$$
\vec{v}(t) =
\begin{pmatrix}
1 \\
-1
\end{pmatrix}
+
\begin{pmatrix}
3 \\
1
\end{pmatrix}
t =
\begin{pmatrix}
1 + 3t \\
-1 + t
\end{pmatrix}
\ \mathrm{\frac{m}{s}}
$$

The position vector is found by integrating the velocity and adding the initial position:

$$
\vec{r}(t) = \vec{r}(0) + \vec{v}(0)t + \frac{1}{2}\vec{a}t^2
$$

$$
\vec{r}(t) =
\begin{pmatrix}
0 \\
0
\end{pmatrix}
+
\begin{pmatrix}
1 \\
-1
\end{pmatrix}
t + \frac{1}{2}
\begin{pmatrix}
3 \\
1
\end{pmatrix}
t^2 =
\begin{pmatrix}
t + 1.5t^2 \\
-t + 0.5t^2
\end{pmatrix}
\ \mathrm{m}
$$

To define the trajectory, the parametric equations are extracted from the position vector:

$$
x(t) = t + 1.5t^2
$$

$$
y(t) = -t + 0.5t^2
$$

To calculate the work done at $t=3\ \mathrm{s}$, the displacement must be computed:

$$
\Delta\vec{r} = \vec{r}(3) - \vec{r}(0) =
\begin{pmatrix}
3 + 1.5(3^2) \\
-3 + 0.5(3^2)
\end{pmatrix}
=
\begin{pmatrix}
3 + 13.5 \\
-3 + 4.5
\end{pmatrix}
=
\begin{pmatrix}
16.5 \\
1.5
\end{pmatrix}
\ \mathrm{m}
$$

The work done is the dot product of the force and the displacement:

$$
W = \vec{F} \cdot \Delta\vec{r} = (6)(16.5) + (2)(1.5)
$$

$$
W = 99 + 3 = 102\ \mathrm{J}
$$

To check the consistency with the work-energy theorem, the initial and final kinetic energies are calculated. The initial kinetic energy is:

$$
T(0) = \frac{1}{2}m |\vec{v}(0)|^2 = \frac{1}{2}(2)(1^2 + (-1)^2) = 2\ \mathrm{J}
$$

The final velocity at $t=3\ \mathrm{s}$ is evaluated:

$$
\vec{v}(3) =
\begin{pmatrix}
1 + 3(3) \\
-1 + 3
\end{pmatrix}
=
\begin{pmatrix}
10 \\
2
\end{pmatrix}
\ \mathrm{\frac{m}{s}}
$$

The final kinetic energy is:

$$
T(3) = \frac{1}{2}m |\vec{v}(3)|^2 = \frac{1}{2}(2)(10^2 + 2^2) = 100 + 4 = 104\ \mathrm{J}
$$

The change in kinetic energy is:

$$
\Delta T = T(3) - T(0) = 104 - 2 = 102\ \mathrm{J}
$$

## Final Result

Acceleration vector:

$$
\vec{a}(t) =
\begin{pmatrix}
3 \\
1
\end{pmatrix}
\ \mathrm{\frac{m}{s^2}}
$$

Velocity vector:

$$
\vec{v}(t) =
\begin{pmatrix}
1 + 3t \\
-1 + t
\end{pmatrix}
\ \mathrm{\frac{m}{s}}
$$

Position vector:

$$
\vec{r}(t) =
\begin{pmatrix}
t + 1.5t^2 \\
-t + 0.5t^2
\end{pmatrix}
\ \mathrm{m}
$$

The work done at $t=3\ \mathrm{s}$ is $102\ \mathrm{J}$. The change in kinetic energy is exactly $102\ \mathrm{J}$.

## Interpretation

The parametric equations describe a parabola in the two-dimensional plane, which is the standard trajectory for a body undergoing constant acceleration with an initial velocity not parallel to the force. The equivalence of the calculated work and the change in kinetic energy confirms the fundamental work-energy theorem for this specific dynamical system.
# Task 02 – Inclined plane with friction

## Problem Statement

A body of mass $m$ slides down an inclined plane with an angle $\alpha$. The coefficient of kinetic friction is $\mu$. Determine all forces acting on the body, derive the acceleration $\vec{a}$, calculate the time of descent from height $h$, determine the final velocity $\vec{v}$, and check if the result is consistent with the energy balance.

## Theory

The body experiences forces that dictate its motion according to Newton's second law. The relevant forces are gravity, the normal force from the surface, and kinetic friction.

Kinetic friction opposes the direction of motion and is proportional to the normal force:

$$
F_k = \mu N
$$

The total mechanical energy $E$ is the sum of kinetic $T$ and potential $U$ energy. The work-energy theorem extended to non-conservative forces states that the work done by friction equals the change in total mechanical energy:

$$
W_{nc} = \Delta E = E_f - E_i
$$

## Step-by-Step Solution

Three primary forces act on the mass $m$:
1. Gravitational force $\vec{F}_g$ pointing strictly downwards.
2. Normal force $\vec{N}$ pointing perpendicular to the inclined plane.
3. Kinetic friction $\vec{F}_k$ pointing parallel to the incline, opposite to the velocity.

A coordinate system is established where the $x$-axis is parallel to the incline pointing downwards, and the $y$-axis is perpendicular to the incline pointing outwards.

The forces are decomposed into these axes. The sum of forces in the $y$-direction is zero since there is no motion perpendicular to the plane:

$$
\sum F_y = N - mg\cos\alpha = 0
$$

$$
N = mg\cos\alpha
$$

The magnitude of the kinetic friction force is determined:

$$
F_k = \mu N = \mu mg\cos\alpha
$$

The equation of motion in the $x$-direction yields the acceleration:

$$
\sum F_x = mg\sin\alpha - F_k = ma
$$

$$
ma = mg\sin\alpha - \mu mg\cos\alpha
$$

Dividing by $m$ yields the constant acceleration:

$$
a = g(\sin\alpha - \mu\cos\alpha)
$$

The body descends from a vertical height $h$. The distance $d$ traveled along the incline is related to $h$ by trigonometry:

$$
\sin\alpha = \frac{h}{d}
$$

$$
d = \frac{h}{\sin\alpha}
$$

Using the kinematic equation for position under constant acceleration from rest:

$$
d = \frac{1}{2}at^2
$$

The time of descent $t$ is calculated:

$$
t = \sqrt{\frac{2d}{a}} = \sqrt{\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}}
$$

The final velocity $v$ at the bottom of the incline is:

$$
v = at = \sqrt{2ad} = \sqrt{2g(\sin\alpha - \mu\cos\alpha)\frac{h}{\sin\alpha}}
$$

To verify the energy balance, the initial and final mechanical energies are evaluated. The initial energy at height $h$ is purely potential:

$$
E_i = mgh
$$

The final energy at the bottom is purely kinetic:

$$
E_f = \frac{1}{2}mv^2
$$

The work done by the non-conservative friction force over distance $d$ is:

$$
W_{nc} = -F_k d = -(\mu mg\cos\alpha) \left( \frac{h}{\sin\alpha} \right) = -\mu mgh\cot\alpha
$$

The expression for $E_f$ is expanded by substituting $v^2$:

$$
\begin{align}
E_f &= \frac{1}{2}m \left( 2g(\sin\alpha - \mu\cos\alpha)\frac{h}{\sin\alpha} \right) \\
    &= mgh \left( \frac{\sin\alpha - \mu\cos\alpha}{\sin\alpha} \right) \\
    &= mgh(1 - \mu\cot\alpha)
\end{align}
$$

The change in total energy is computed:

$$
\begin{align}
\Delta E &= E_f - E_i \\
         &= mgh(1 - \mu\cot\alpha) - mgh \\
         &= -\mu mgh\cot\alpha
\end{align}
$$

## Final Result

The acceleration is:

$$
a = g(\sin\alpha - \mu\cos\alpha)
$$

The time of descent is:

$$
t = \sqrt{\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}}
$$

The final velocity is:

$$
v = \sqrt{2gh(1 - \mu\cot\alpha)}
$$

The change in energy $\Delta E = -\mu mgh\cot\alpha$ perfectly matches the work done by friction $W_{nc}$.

## Interpretation

The presence of kinetic friction explicitly reduces the net acceleration, thereby increasing the descent time and reducing the final velocity compared to a frictionless surface. The mechanical energy dissipated as thermal energy perfectly matches the negative work done by the non-conservative frictional force, verifying the generalized conservation of energy.

# Task 03 – Work of a variable force

## Problem Statement

Given a one-dimensional force:

$$
F(x) = -kx
$$

Write down the equation of motion and solve it. Calculate the work done during the displacement from $0$ to $x_0$. Interpret the result as potential energy, verify the relationship $F = -\frac{dU}{dx}$, and draw the graph of $F(x)$ and $U(x)$.

## Theory

The force provided follows Hooke's Law, representing a linear restoring force. This creates a dynamical system known as a simple harmonic oscillator.

The work done by a variable one-dimensional force is defined by the integral:

$$
W = \int_{x_i}^{x_f} F(x) \, dx
$$

For a conservative force, the change in potential energy is the negative of the work done by that force:

$$
\Delta U = -W
$$

This leads to the differential relationship between force and potential energy:

$$
F(x) = -\frac{dU}{dx}
$$

## Step-by-Step Solution

The equation of motion is constructed using Newton's second law:

$$
m\ddot{x} = -kx
$$

$$
\ddot{x} + \frac{k}{m}x = 0
$$

By defining the angular frequency $\omega = \sqrt{\frac{k}{m}}$, the equation becomes a standard second-order linear homogeneous differential equation:

$$
\ddot{x} + \omega^2 x = 0
$$

The general solution to this differential equation is:

$$
x(t) = A\cos(\omega t + \phi)
$$

where $A$ is the amplitude and $\phi$ is the phase constant, determined by initial conditions.

The work done by the force $F(x)$ during displacement from the origin to a position $x_0$ is evaluated via integration:

$$
W = \int_{0}^{x_0} F(x) \, dx = \int_{0}^{x_0} (-kx) \, dx
$$

$$
W = \left[ -\frac{1}{2}kx^2 \right]_0^{x_0} = -\frac{1}{2}kx_0^2
$$

The potential energy function $U(x)$ is derived by utilizing the definition $\Delta U = -W$. Setting the reference potential energy at the origin to zero, $U(0) = 0$:

$$
U(x_0) - U(0) = -\left( -\frac{1}{2}kx_0^2 \right)
$$

$$
U(x_0) = \frac{1}{2}kx_0^2
$$

Replacing the specific coordinate $x_0$ with a general coordinate $x$ gives the potential energy function:

$$
U(x) = \frac{1}{2}kx^2
$$

The inverse relationship is verified by differentiating the derived potential energy with respect to position:

$$
-\frac{dU}{dx} = -\frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = -kx
$$

## Final Result

The equation of motion is $m\ddot{x} + kx = 0$, and its solution is:

$$
x(t) = A\cos\left(\sqrt{\frac{k}{m}}t + \phi\right)
$$

The work done from $0$ to $x_0$ is:

$$
W = -\frac{1}{2}kx_0^2
$$

The potential energy function is:

$$
U(x) = \frac{1}{2}kx^2
$$

The gradient derivative correctly returns the initial force $F(x) = -kx$.

## Interpretation

The graph of $F(x)$ is a straight line passing through the origin with a negative slope $-k$, demonstrating that the force always points opposite to the displacement. The graph of $U(x)$ is an upward-opening parabola with its vertex at the origin. This quadratic potential energy well traps the particle, causing it to continuously exchange kinetic and potential energy, resulting in the oscillatory periodic motion described by the solution $x(t)$.
# Task 04 – Conservation of energy

## Problem Statement

A body falls from a height $h$ without air resistance. Write down the total energy $E(h) = T(h) + U(h)$ and determine the velocity as a function of height $v(h)$. Compare with the solution from Newton's second law. At what height does the kinetic energy account for 75% of the total energy?

## Theory

For an object moving strictly under the influence of conservative forces (like gravity), total mechanical energy is conserved:

$$
E_i = E_f
$$

The total energy $E$ is the sum of the kinetic energy $T = \frac{1}{2}mv^2$ and the gravitational potential energy $U = mgy$.

Newton's second law allows an alternative kinematic derivation of velocity by integrating the constant acceleration due to gravity.

## Step-by-Step Solution

The body is dropped from rest at a vertical position $y = h$. The initial kinetic energy is zero, and the potential energy is maximized. The total initial energy is:

$$
E(h) = T(h) + U(h) = 0 + mgh = mgh
$$

As the body falls to an arbitrary height $y$, its total energy remains identical to the initial energy. The energy balance is written as:

$$
E(y) = \frac{1}{2}mv^2 + mgy = mgh
$$

The velocity $v$ as a function of height $y$ is isolated:

$$
\frac{1}{2}mv^2 = mg(h - y)
$$

$$
v(y) = \sqrt{2g(h - y)}
$$

To compare this with Newton's second law, the equation of motion in the vertical axis is constructed:

$$
m\ddot{y} = -mg
$$

$$
a = \ddot{y} = -g
$$

Using the time-independent kinematic relation for constant acceleration $v^2 = v_0^2 + 2a(y - y_0)$, with initial velocity $v_0 = 0$ at position $y_0 = h$:

$$
v^2 = 0 + 2(-g)(y - h) = 2g(h - y)
$$

$$
v(y) = \sqrt{2g(h - y)}
$$

The results are identical.

Next, the height where the kinetic energy accounts for 75% of the total mechanical energy is computed:

$$
T = 0.75 E
$$

Since $E = T + U$, this requires the potential energy to account for the remaining 25% of the total energy:

$$
U = 0.25 E
$$

Substituting the known forms of potential and total energy:

$$
mgy = 0.25 (mgh)
$$

$$
y = 0.25 h = \frac{1}{4}h
$$

## Final Result

The total energy of the system is constant and equals $mgh$. The velocity as a function of height is:

$$
v(y) = \sqrt{2g(h - y)}
$$

This fully matches the solution derived from Newton's second law. The kinetic energy reaches 75% of the total energy at the height:

$$
y = \frac{1}{4}h
$$

## Interpretation

The derivation shows the exact equivalence between the energy approach and the direct integration of Newton's equations of motion. Energy methods inherently provide a scalar, path-independent way to determine velocity as a direct function of position, completely bypassing the need to explicitly solve for time.
# Task 05 – Momentum and one-dimensional head-on collision

## Problem Statement

Two bodies with masses $m_1$ and $m_2$ move along a single straight line. The collision is perfectly elastic. Write down the principles of conservation of momentum and energy. Determine the velocities after the collision. Consider the case $m_1 = m_2$ and the limit $m_2 \gg m_1$. Interpret the results physically.

## Theory

For an isolated system with no external forces, the total momentum is conserved. If the collision is perfectly elastic, the total kinetic energy of the system is also conserved. 

Let $v_1$ and $v_2$ be the initial velocities of masses $m_1$ and $m_2$ respectively, and $u_1$ and $u_2$ be their final velocities after the collision.

The principle of conservation of momentum is:

$$
m_1 v_1 + m_2 v_2 = m_1 u_1 + m_2 u_2
$$

The principle of conservation of kinetic energy is:

$$
\frac{1}{2}m_1 v_1^2 + \frac{1}{2}m_2 v_2^2 = \frac{1}{2}m_1 u_1^2 + \frac{1}{2}m_2 u_2^2
$$

## Step-by-Step Solution

To find the final velocities $u_1$ and $u_2$, the conservation equations are rearranged. First, group the terms associated with each mass.

From the momentum equation:

$$
m_1(v_1 - u_1) = m_2(u_2 - v_2)
$$

From the kinetic energy equation (multiplying by 2 first):

$$
m_1(v_1^2 - u_1^2) = m_2(u_2^2 - v_2^2)
$$

Using the difference of squares factorization on the energy equation:

$$
m_1(v_1 - u_1)(v_1 + u_1) = m_2(u_2 - v_2)(u_2 + v_2)
$$

Assuming a non-trivial collision ($v_1 \neq u_1$ and $v_2 \neq u_2$), divide
# Task 06 – Motion with linear drag

## Problem Statement

The drag force acting on a moving body is given by the formula $F = -kv$. The initial conditions are $v(0)=v_0$ and $x(0)=0$. Write down the equation of motion and solve it. Investigate the limit $\lim_{t\to\infty} v(t)$ and compare it with motion without drag.

## Theory

A drag force proportional to velocity is typical for objects moving slowly through a viscous fluid (Stokes' drag). Newton's second law provides the equation of motion. Since the force depends strictly on velocity, the resulting differential equation is a first-order separable ordinary differential equation (ODE) in terms of velocity.

## Step-by-Step Solution

Applying Newton's second law:

$$
m\frac{dv}{dt} = -kv
$$

This equation is solved by separation of variables:

$$
\frac{dv}{v} = -\frac{k}{m}dt
$$

Integrating both sides from the initial state ($t=0$, $v=v_0$) to an arbitrary state ($t$, $v(t)$):

$$
\int_{v_0}^{v(t)} \frac{1}{v'} \, dv' = \int_0^t -\frac{k}{m} \, dt'
$$

$$
\ln(v(t)) - \ln(v_0) = -\frac{k}{m}t
$$

$$
\ln\left(\frac{v(t)}{v_0}\right) = -\frac{k}{m}t
$$

Exponentiating both sides yields the velocity function:

$$
v(t) = v_0 e^{-\frac{k}{m}t}
$$

To find the position as a function of time, substitute $v(t) = \frac{dx}{dt}$ and integrate again:

$$
dx = v_0 e^{-\frac{k}{m}t} \, dt
$$

Integrating from $x(0) = 0$ to $x(t)$:

$$
\int_0^{x(t)} dx' = \int_0^t v_0 e^{-\frac{k}{m}t'} \, dt'
$$

$$
x(t) = \left[ -\frac{m v_0}{k} e^{-\frac{k}{m}t'} \right]_0^t
$$

$$
x(t) = -\frac{m v_0}{k} \left( e^{-\frac{k}{m}t} - 1 \right) = \frac{m v_0}{k} \left( 1 - e^{-\frac{k}{m}t} \right)
$$

Next, investigate the limit of the velocity as time approaches infinity:

$$
\lim_{t\to\infty} v(t) = \lim_{t\to\infty} v_0 e^{-\frac{k}{m}t} = 0
$$

We can also evaluate the maximum distance traveled (stopping distance) by taking the limit of $x(t)$:

$$
x_{max} = \lim_{t\to\infty} \frac{m v_0}{k} \left( 1 - e^{-\frac{k}{m}t} \right) = \frac{m v_0}{k}
$$

## Final Result

The equation of motion is $m\dot{v} = -kv$. The exact solutions are:

$$
v(t) = v_0 e^{-\frac{k}{m}t}
$$

$$
x(t) = \frac{m v_0}{k} \left( 1 - e^{-\frac{k}{m}t} \right)
$$

The asymptotic limits are:

$$
\lim_{t\to\infty} v(t) = 0
$$

$$
\lim_{t\to\infty} x(t) = \frac{m v_0}{k}
$$

## Interpretation

The velocity decays exponentially over time due to the continuous dissipation of kinetic energy by the viscous drag force. The object never completely stops mathematically in finite time, but its velocity rapidly approaches zero. 

By comparison, a body in motion without any drag force ($k=0$) would maintain a constant velocity $v(t) = v_0$ indefinitely, and its position $x(t) = v_0 t$ would grow linearly without bound. The presence of linear drag bounds the total distance the object can travel to a finite limit $x_{max}$, which is directly proportional to mass and initial velocity, and inversely proportional to the drag coefficient.
# Task 07 – Vertical throw with drag

## Problem Statement

We have the equation of motion $m\frac{dv}{dt} = -mg - kv$ with initial conditions $v(0)=v_0$ and $x(0)=0$. Solve the equation, determine the maximum height, compare with the case without drag, perform a numerical simulation conceptually, and compare the analytical and numerical solutions.

## Theory

A vertical throw in a viscous medium involves two forces: the constant downward force of gravity and a velocity-dependent drag force opposing the motion. The equation is a non-homogeneous first-order linear ordinary differential equation. 

The analytical solution provides exact continuous functions for velocity and position. A numerical approach utilizes discrete time steps to approximate the differential changes in state variables, essential for validating complex systems or handling non-linear drag where exact analytical solutions do not exist.

## Step-by-Step Solution

The equation of motion is separated:

$$
\frac{dv}{dt} = -g - \frac{k}{m}v = -\frac{k}{m} \left( \frac{mg}{k} + v \right)
$$

Let the terminal velocity be defined as $v_t = \frac{mg}{k}$. The equation becomes:

$$
\frac{dv}{v_t + v} = -\frac{k}{m}dt
$$

Integrating from $v(0) = v_0$ to $v(t)$:

$$
\int_{v_0}^{v(t)} \frac{dv'}{v_t + v'} = \int_0^t -\frac{k}{m} \, dt'
$$

$$
\ln\left( \frac{v_t + v(t)}{v_t + v_0} \right) = -\frac{k}{m}t
$$

Exponentiating and solving for $v(t)$:

$$
v_t + v(t) = (v_t + v_0) e^{-\frac{k}{m}t}
$$

$$
v(t) = (v_t + v_0) e^{-\frac{k}{m}t} - v_t
$$

To find the position $x(t)$, integrate the velocity function from $x(0)=0$ to $x(t)$:

$$
x(t) = \int_0^t \left[ (v_t + v_0) e^{-\frac{k}{m}t'} - v_t \right] \, dt'
$$

$$
x(t) = \left[ -\frac{m}{k}(v_t + v_0) e^{-\frac{k}{m}t'} - v_t t' \right]_0^t
$$

$$
\begin{align}
x(t) &= -\frac{m}{k}(v_t + v_0) e^{-\frac{k}{m}t} - v_t t - \left( -\frac{m}{k}(v_t + v_0) \right) \\
     &= \frac{m}{k}(v_t + v_0) \left( 1 - e^{-\frac{k}{m}t} \right) - v_t t
\end{align}
$$

The maximum height $h$ is reached at time $t_1$ when the velocity is zero ($v(t_1) = 0$):

$$
0 = (v_t + v_0) e^{-\frac{k}{m}t_1} - v_t
$$

$$
e^{\frac{k}{m}t_1} = \frac{v_t + v_0}{v_t} = 1 + \frac{v_0}{v_t}
$$

$$
t_1 = \frac{m}{k} \ln\left( 1 + \frac{v_0}{v_t} \right)
$$

Substituting $t_1$ into the position equation, noting that $e^{-\frac{k}{m}t_1} = \frac{v_t}{v_t + v_0}$:

$$
h = x(t_1) = \frac{m}{k}(v_t + v_0) \left( 1 - \frac{v_t}{v_t + v_0} \right) - v_t \left( \frac{m}{k} \ln\left( 1 + \frac{v_0}{v_t} \right) \right)
$$

$$
h = \frac{m v_0}{k} - \frac{m v_t}{k} \ln\left( 1 + \frac{v_0}{v_t} \right)
$$

**Numerical Simulation (Euler Method):**
To solve the system numerically, the time domain is discretized into steps of $\Delta t$. The continuous derivatives are approximated by finite differences:

$$
v_{n+1} = v_n + \left( -g - \frac{k}{m}v_n \right) \Delta t
$$

$$
x_{n+1} = x_n + v_n \Delta t
$$

Starting with $x_0 = 0$ and $v_0$, iterative calculation yields a sequence of states $(x_n, v_n)$ representing the trajectory over time.

## Final Result

The analytical velocity and position functions are:

$$
v(t) = \left( \frac{mg}{k} + v_0 \right) e^{-\frac{k}{m}t} - \frac{mg}{k}
$$

$$
x(t) = \frac{m}{k}\left( \frac{mg}{k} + v_0 \right) \left( 1 - e^{-\frac{k}{m}t} \right) - \frac{mg}{k} t
$$

The maximum height reached is:

$$
h = \frac{m v_0}{k} - \frac{m^2 g}{k^2} \ln\left( 1 + \frac{k v_0}{mg} \right)
$$

Without drag, the standard kinematic maximum height is strictly $h_{no\_drag} = \frac{v_0^2}{2g}$.

## Interpretation

The drag force constantly acts opposite to the direction of motion, compounding with gravity during the ascent. Consequently, the maximum height $h$ achieved is strictly lower than $h_{no\_drag}$. The logarithmic term subtracts heavily from the ideal trajectory.

The analytical solution provides the exact coordinates for the body at any arbitrary time, but solving for specific variables often requires isolating transcendental roots. The numerical Euler simulation is highly accessible and easily adaptable, allowing the physical trajectory to be graphed by a computer step-by-step. As the time step $\Delta t$ approaches zero, the numerical solution converges directly to the exact analytical curves derived above.
# Task 08 – Harmonic oscillator (formal dynamics)

## Problem Statement

Consider the differential equation:

$$
m\ddot{x} + kx = 0
$$

Solve the equation, determine the natural frequency, write down the energy as a function of time, show that energy is conserved, and interpret the motion in phase space.

## Theory

The given equation describes a simple harmonic oscillator, where a restoring force proportional to the displacement acts on a mass $m$. The restoring force constant is $k$. 

This is a second-order, linear, homogeneous ordinary differential equation. The natural frequency defines the rate of oscillation inherent to the system based on its mass and stiffness. The phase space represents the dynamical state of the system through coordinate pairs of position and momentum (or position and velocity), offering a geometric interpretation of the motion.

## Step-by-Step Solution

The equation of motion is rewritten in standard form by dividing by the mass $m$:

$$
\ddot{x} + \frac{k}{m}x = 0
$$

The angular natural frequency $\omega_0$ is defined as:

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Substituting the natural frequency, the differential equation becomes:

$$
\ddot{x} + \omega_0^2 x = 0
$$

The general solution to this characteristic equation is a sinusoidal function:

$$
x(t) = A\cos(\omega_0 t + \phi)
$$

where $A$ is the amplitude and $\phi$ is the initial phase, both determined by initial conditions. The velocity is the time derivative of position:

$$
v(t) = \dot{x}(t) = -A\omega_0\sin(\omega_0 t + \phi)
$$

The total mechanical energy $E(t)$ is the sum of kinetic energy $T(t)$ and potential energy $U(t)$:

$$
E(t) = T(t) + U(t) = \frac{1}{2}mv(t)^2 + \frac{1}{2}kx(t)^2
$$

Substituting the time-dependent functions for position and velocity into the energy equation:

$$
E(t) = \frac{1}{2}m\left(-A\omega_0\sin(\omega_0 t + \phi)\right)^2 + \frac{1}{2}k\left(A\cos(\omega_0 t + \phi)\right)^2
$$

$$
E(t) = \frac{1}{2}mA^2\omega_0^2\sin^2(\omega_0 t + \phi) + \frac{1}{2}kA^2\cos^2(\omega_0 t + \phi)
$$

Recall that $\omega_0^2 = \frac{k}{m}$, which implies $m\omega_0^2 = k$. Substituting this into the kinetic energy term:

$$
\begin{align}
E(t) &= \frac{1}{2}kA^2\sin^2(\omega_0 t + \phi) + \frac{1}{2}kA^2\cos^2(\omega_0 t + \phi) \\
     &= \frac{1}{2}kA^2 \left( \sin^2(\omega_0 t + \phi) + \cos^2(\omega_0 t + \phi) \right)
\end{align}
$$

Using the Pythagorean trigonometric identity $\sin^2(\theta) + \cos^2(\theta) = 1$, the time dependence vanishes:

$$
E(t) = \frac{1}{2}kA^2
$$

Because the total energy $E(t)$ depends only on the constant system parameters ($k$) and initial conditions ($A$), and has no explicit time dependence, the energy is strictly conserved.

To interpret the motion in phase space, we use the coordinates $(x, v)$. From the solutions for $x(t)$ and $v(t)$, we can isolate the trigonometric terms:

$$
\cos(\omega_0 t + \phi) = \frac{x}{A}
$$

$$
\sin(\omega_0 t + \phi) = -\frac{v}{A\omega_0}
$$

Squaring and adding these equations eliminates time, yielding the phase space trajectory:

$$
\left(\frac{x}{A}\right)^2 + \left(\frac{v}{A\omega_0}\right)^2 = 1
$$

## Final Result

The general solution is:

$$
x(t) = A\cos\left(\sqrt{\frac{k}{m}}t + \phi\right)
$$

The natural frequency is:

$$
f_0 = \frac{\omega_0}{2\pi} = \frac{1}{2\pi}\sqrt{\frac{k}{m}}
$$

The total energy is conserved and strictly equals:

$$
E = \frac{1}{2}kA^2
$$

The phase space trajectory is defined by the equation of an ellipse.

## Interpretation

The exact conservation of energy is a direct consequence of the restoring force being perfectly conservative. In the $(x, v)$ phase space, the state of the system traces a closed elliptical path continuously. A closed loop in phase space strictly indicates periodic, bounded motion. The semi-major and semi-minor axes of the ellipse are $A$ and $A\omega_0$, directly scaling with the total energy of the system.
# Task 09 – Potential and conservative field

## Problem Statement

Given the potential energy function:

$$
U(x,y) = \frac{k}{2}(x^2+y^2)
$$

Determine the force as the gradient of the potential. Write down the equations of motion. Determine the type of motion. Determine the total energy. Interpret the trajectory geometrically, presenting it in an HTML/JS application context.

## Theory

For a conservative force field, the force vector $\vec{F}$ is the negative gradient of the scalar potential energy field $U$:

$$
\vec{F} = -\nabla U =
\begin{pmatrix}
-\frac{\partial U}{\partial x} \\
-\frac{\partial U}{\partial y}
\end{pmatrix}
$$

Newton's second law applied to each spatial dimension yields a system of coupled or uncoupled differential equations. The total energy is the sum of the kinetic and potential energies in all dimensions.

## Step-by-Step Solution

The components of the force vector are obtained by taking the partial derivatives of the potential energy $U(x,y)$:

$$
F_x = -\frac{\partial}{\partial x} \left[ \frac{k}{2}(x^2+y^2) \right] = -kx
$$

$$
F_y = -\frac{\partial}{\partial y} \left[ \frac{k}{2}(x^2+y^2) \right] = -ky
$$

The force vector is:

$$
\vec{F} =
\begin{pmatrix}
-kx \\
-ky
\end{pmatrix}
= -k
\begin{pmatrix}
x \\
y
\end{pmatrix}
= -k\vec{r}
$$

The equations of motion are written applying $m\vec{a} = \vec{F}$:

$$
m\ddot{x} = -kx
$$

$$
m\ddot{y} = -ky
$$

Dividing by $m$ yields two independent harmonic oscillator equations:

$$
\ddot{x} + \frac{k}{m}x = 0
$$

$$
\ddot{y} + \frac{k}{m}y = 0
$$

Defining $\omega_0 = \sqrt{\frac{k}{m}}$, the solutions are independent oscillations in the $x$ and $y$ directions:

$$
x(t) = A_x \cos(\omega_0 t + \phi_x)
$$

$$
y(t) = A_y \cos(\omega_0 t + \phi_y)
$$

The total mechanical energy $E$ is the sum of the kinetic energy in both directions and the total potential energy:

$$
E = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}m\dot{y}^2 + \frac{k}{2}(x^2+y^2)
$$

Since the motions in $x$ and $y$ are independent harmonic oscillators, the energy in each axis is conserved independently:

$$
E_x = \frac{1}{2}k A_x^2
$$

$$
E_y = \frac{1}{2}k A_y^2
$$

The total energy is simply their sum:

$$
E = E_x + E_y = \frac{1}{2}k(A_x^2 + A_y^2)
$$

To interpret the trajectory geometrically, consider the parametric equations $x(t)$ and $y(t)$. Because both axes oscillate with the exact same frequency $\omega_0$, the resulting path in the $xy$-plane is generally an ellipse, characterized by the relative phase difference $\delta = \phi_y - \phi_x$ and the amplitudes $A_x, A_y$. 

If $\delta = 0$ or $\delta = \pi$, the ellipse degenerates into a straight line. If $A_x = A_y$ and $\delta = \pm \pi/2$, the ellipse becomes a perfect circle.

## Final Result

The force vector is a central restoring force:

$$
\vec{F} = -k\vec{r}
$$

The equations of motion are uncoupled:

$$
\ddot{x} + \frac{k}{m}x = 0
$$

$$
\ddot{y} + \frac{k}{m}y = 0
$$

The system exhibits motion equivalent to a 2D isotropic harmonic oscillator. The total energy is constant:

$$
E = \frac{1}{2}k(A_x^2 + A_y^2)
$$

## Interpretation

The central potential $U(x,y)$ creates a 2D isotropic harmonic oscillator, representing a mass attached to a fixed origin by a spring satisfying Hooke's Law in two dimensions. 

In an HTML/JS simulation, you would use a standard `requestAnimationFrame` loop. You would initialize variables for time `t`, evaluate `x = Ax * Math.cos(w * t + px)` and `y = Ay * Math.cos(w * t + py)`, and draw a line segment from the previous `(x, y)` coordinate to the new one on a `<canvas>` element. Tweaking the phase difference and amplitude sliders in the UI would smoothly deform the rendered geometric trajectory between straight lines, slanted ellipses, and circles (Lissajous figures for a 1:1 frequency ratio).
# Task 10 – Numerical model of a dynamical system

## Problem Statement

Consider motion in a one-dimensional potential:

$$
U(x) = \frac{k}{2}x^2 + \lambda x^4
$$

Determine the force, write down the equation of motion, formulate a numerical solution for selected parameters, investigate the effect of initial energy on the type of motion, and describe the visualization of $x(t)$ and the phase portrait.

## Theory

This potential represents an anharmonic oscillator (specifically, the Duffing oscillator without damping or driving). The linear term $\frac{k}{2}x^2$ provides standard harmonic restitution, while the non-linear $\lambda x^4$ term alters the stiffness at larger displacements. If $\lambda > 0$, the spring is "hardening" (stiffness increases with displacement). 

Due to the non-linear nature of the force, exact elementary analytical solutions do not exist, making numerical integration techniques (such as Euler-Cromer or Runge-Kutta) necessary to determine the trajectory over time.

## Step-by-Step Solution

The conservative force is the negative derivative of the potential energy:

$$
F(x) = -\frac{dU}{dx} = -\frac{d}{dx}\left( \frac{k}{2}x^2 + \lambda x^4 \right)
$$

$$
F(x) = -kx - 4\lambda x^3
$$

Using Newton's second law, the equation of motion is:

$$
m\ddot{x} = -kx - 4\lambda x^3
$$

$$
\ddot{x} + \frac{k}{m}x + \frac{4\lambda}{m}x^3 = 0
$$

To solve this numerically, the second-order ordinary differential equation must be decomposed into a system of two coupled first-order equations. Let the velocity be $v = \dot{x}$:

$$
\frac{dx}{dt} = v
$$

$$
\frac{dv}{dt} = -\frac{k}{m}x - \frac{4\lambda}{m}x^3
$$

Given a small time step $\Delta t$, the state variables are updated iteratively. Using the semi-implicit Euler method (Euler-Cromer) which perfectly conserves energy for oscillatory systems over long periods:

$$
v_{n+1} = v_n + \left( -\frac{k}{m}x_n - \frac{4\lambda}{m}x_n^3 \right)\Delta t
$$

$$
x_{n+1} = x_n + v_{n+1}\Delta t
$$

The initial energy $E_0$ dictates the amplitude of motion and heavily influences the dynamics:

$$
E_0 = \frac{1}{2}mv_0^2 + \frac{k}{2}x_0^2 + \lambda x_0^4
$$

**Low Energy Limit:**
For small initial energy, the maximum displacement $x$ remains small. Because $x^3 \ll x$ when $x$ is near zero, the non-linear term $4\lambda x^3$ becomes negligible. The system behaves almost exactly like a simple harmonic oscillator. The motion is sinusoidal, and the frequency is approximately $\omega_0 = \sqrt{k/m}$, independent of amplitude.

**High Energy Limit:**
For massive initial energy, the displacement becomes large, and the non-linear term dominates ($4\lambda x^3 \gg kx$). Assuming $\lambda > 0$, the restoring force increases faster than a linear spring. This causes the body to accelerate back to the equilibrium point much faster than in a harmonic oscillator. Consequently, the period of oscillation strictly decreases (frequency increases) as the initial energy and amplitude increase. The motion is periodic but fundamentally non-sinusoidal.

## Final Result

The continuous non-linear force is:

$$
F(x) = -kx - 4\lambda x^3
$$

The equation of motion is:

$$
\ddot{x} + \frac{k}{m}x + \frac{4\lambda}{m}x^3 = 0
$$

The numerical integration relies on the first-order system:

$$
\dot{x} = v
$$

$$
\dot{v} = -\frac{k}{m}x - \frac{4\lambda}{m}x^3
$$

## Interpretation

In visualizing $x(t)$, low energy initial states yield a standard sine wave graph. High energy initial states (with $\lambda > 0$) yield a periodic wave that appears sharper at the peaks and flatter at the zero-crossings compared to a sine wave, demonstrating the amplitude-dependent frequency.

In the phase portrait $(x, v)$, a low energy trajectory traces a pure ellipse. As energy increases, the non-linear term distorts the phase portrait trajectory. For a hardening spring ($\lambda > 0$), the ellipse is stretched vertically, taking on an increasingly squarish or "peanut-like" shape, reflecting the rapid velocity changes at high displacements. Unlike chaotic systems, because energy is conserved and there are no driving forces, the phase portrait remains a closed, strictly periodic loop for any non-zero initial energy.