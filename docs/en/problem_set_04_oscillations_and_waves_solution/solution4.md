# Task 01 – Harmonic motion: motion parameters

## Problem Statement

A function describing harmonic motion is given by

$$
x(t) = A \cos(\omega t + \varphi)
$$

Determine the period $T$, the frequency $f$, the maximum velocity, and the maximum acceleration. Calculate $\omega$, $v_{\max}$, and $a_{\max}$ given $A = 0.2\ \mathrm{m}$ and $f = 2\ \mathrm{Hz}$.

## Theory

Harmonic motion is characterized by an oscillating position coordinate $x(t)$, where $A$ is the amplitude, $\omega$ is the angular frequency, and $\varphi$ is the initial phase. The relationship between angular frequency, period, and linear frequency is governed by basic kinematics of oscillatory systems. Velocity and acceleration are the first and second time derivatives of position, respectively.

## Step-by-Step Solution

The period $T$ is the time required for one complete oscillation. By definition of the cosine function's period, this occurs when the phase changes by $2\pi$:

$$
\omega T = 2\pi
$$

Solving for $T$ yields

$$
T = \frac{2\pi}{\omega}
$$

The frequency $f$ is the reciprocal of the period:

$$
f = \frac{1}{T} = \frac{\omega}{2\pi}
$$

To find the velocity, we take the first derivative of position with respect to time:

$$
\begin{align}
v(t) &= \frac{dx}{dt} \\
     &= \frac{d}{dt} [A \cos(\omega t + \varphi)] \\
     &= -A \omega \sin(\omega t + \varphi)
\end{align}
$$

The maximum magnitude of the velocity occurs when the sine function equals $\pm 1$:

$$
v_{\max} = A \omega
$$

To find the acceleration, we take the second time derivative (or the first derivative of velocity):

$$
\begin{align}
a(t) &= \frac{dv}{dt} \\
     &= \frac{d}{dt} [-A \omega \sin(\omega t + \varphi)] \\
     &= -A \omega^2 \cos(\omega t + \varphi)
\end{align}
$$

The maximum magnitude of the acceleration occurs when the cosine function equals $\pm 1$:

$$
a_{\max} = A \omega^2
$$

For the specific case where $A = 0.2\ \mathrm{m}$ and $f = 2\ \mathrm{Hz}$, we first calculate $\omega$:

$$
\omega = 2\pi f = 2\pi(2) = 4\pi\ \mathrm{rad/s}
$$

Next, we substitute $\omega$ and $A$ into the maximum velocity expression:

$$
v_{\max} = 0.2 \times 4\pi = 0.8\pi\ \mathrm{m/s} \approx 2.51\ \mathrm{m/s}
$$

Finally, we calculate the maximum acceleration:

$$
a_{\max} = 0.2 \times (4\pi)^2 = 0.2 \times 16\pi^2 = 3.2\pi^2\ \mathrm{m/s^2} \approx 31.58\ \mathrm{m/s^2}
$$

## Final Result

The formulas for the parameters are:

$$
T = \frac{2\pi}{\omega}
$$

$$
f = \frac{\omega}{2\pi}
$$

$$
v_{\max} = A\omega
$$

$$
a_{\max} = A\omega^2
$$

The calculated numerical values are:

$$
\omega = 4\pi\ \mathrm{rad/s}
$$

$$
v_{\max} = 0.8\pi\ \mathrm{m/s}
$$

$$
a_{\max} = 3.2\pi^2\ \mathrm{m/s^2}
$$

## Interpretation

The velocity is out of phase with the position by $\pi/2$, meaning the object moves fastest as it crosses the equilibrium point and stops momentarily at the maximum displacement. The acceleration is completely out of phase with the position (by $\pi$), indicating that the restoring force is always directed opposite to the displacement and is strongest at the turning points.
# Task 02 – Energy of a harmonic oscillator

## Problem Statement

A system has the parameters $m = 1\ \mathrm{kg}$, $k = 100\ \mathrm{N/m}$, $x(0) = 2\ \mathrm{m}$, and $v(0) = 1\ \mathrm{m/s}$. Determine the natural frequency, total energy, and the displacement at which kinetic energy constitutes 50% of the total energy.

## Theory

A simple harmonic oscillator consists of a mass $m$ subjected to a linear restoring force described by Hooke's Law, $F = -kx$. The natural angular frequency is dictated by the mass and the spring constant. The total mechanical energy $E$ is conserved and is the sum of kinetic energy $E_k$ and potential energy $E_p$:

$$
E_k = \frac{1}{2} m v^2
$$

$$
E_p = \frac{1}{2} k x^2
$$

$$
E = E_k + E_p
$$

## Step-by-Step Solution

The natural angular frequency $\omega_0$ is given by the square root of the ratio of the spring constant to the mass:

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Substituting the given values:

$$
\omega_0 = \sqrt{\frac{100}{1}} = 10\ \mathrm{rad/s}
$$

The linear frequency $f$ is:

$$
f = \frac{\omega_0}{2\pi} = \frac{10}{2\pi} \approx 1.59\ \mathrm{Hz}
$$

To find the total energy, we evaluate the system at $t = 0$ using the initial conditions:

$$
E = \frac{1}{2} m v(0)^2 + \frac{1}{2} k x(0)^2
$$

Substitute the numerical values:

$$
\begin{align}
E &= \frac{1}{2}(1)(1)^2 + \frac{1}{2}(100)(2)^2 \\
  &= 0.5 + 200 \\
  &= 200.5\ \mathrm{J}
\end{align}
$$

We must find the displacement $x$ where $E_k = 0.5 E$. Since total energy is conserved, this also implies that potential energy accounts for the other 50% of the total energy:

$$
E_p = 0.5 E
$$

Substituting the potential energy formula:

$$
\frac{1}{2} k x^2 = 0.5 E
$$

Isolate $x$:

$$
x^2 = \frac{E}{k}
$$

$$
x = \pm \sqrt{\frac{E}{k}}
$$

Substitute the numerical values:

$$
x = \pm \sqrt{\frac{200.5}{100}} = \pm \sqrt{2.005} \approx \pm 1.416\ \mathrm{m}
$$

## Final Result

The natural angular frequency is

$$
\omega_0 = 10\ \mathrm{rad/s}
$$

The total mechanical energy is

$$
E = 200.5\ \mathrm{J}
$$

The displacement where kinetic energy is 50% of the total energy is

$$
x \approx \pm 1.416\ \mathrm{m}
$$

## Interpretation

The total mechanical energy is fixed entirely by the initial state of the system. Energy constantly shifts back and forth between the kinetic store (associated with motion) and the potential store (associated with spring deformation). At $x \approx \pm 1.416\ \mathrm{m}$, the energy is partitioned exactly equally between the two forms.
# Task 03 – Harmonic wave

## Problem Statement

A harmonic wave is defined by

$$
y(x,t) = A \sin(kx - \omega t)
$$

Determine the wavelength and phase velocity. Calculate the velocity for $k = 4\pi$ and $\omega = 20\pi$. Determine if the point $x = \lambda$ oscillates in phase with the point $x = 0$.

## Theory

A one-dimensional harmonic wave represents a periodic disturbance propagating through space. The argument $kx - \omega t$ is the phase of the wave, where $k$ is the wavenumber and $\omega$ is the angular frequency. Points of constant phase move forward at the phase velocity $v$.

## Step-by-Step Solution

The wavenumber $k$ represents spatial frequency, relating to wavelength $\lambda$ in the same way $\omega$ relates to period $T$:

$$
k = \frac{2\pi}{\lambda}
$$

Rearranging for $\lambda$ yields

$$
\lambda = \frac{2\pi}{k}
$$

The phase velocity $v$ is the speed at which a point of constant phase propagates. If we set $kx - \omega t = \text{constant}$ and differentiate with respect to time $t$, we obtain

$$
k \frac{dx}{dt} - \omega = 0
$$

Since $dx/dt$ is the phase velocity $v$, we have

$$
v = \frac{\omega}{k}
$$

Using the given values $k = 4\pi\ \mathrm{m^{-1}}$ and $\omega = 20\pi\ \mathrm{rad/s}$, we compute the phase velocity:

$$
v = \frac{20\pi}{4\pi} = 5\ \mathrm{m/s}
$$

To check the phase alignment, we substitute $x = 0$ into the wave equation:

$$
y(0,t) = A \sin(-\omega t) = -A \sin(\omega t)
$$

Now we evaluate the wave equation at $x = \lambda$:

$$
y(\lambda,t) = A \sin(k\lambda - \omega t)
$$

Substitute $k = 2\pi / \lambda$:

$$
\begin{align}
y(\lambda,t) &= A \sin\left(\frac{2\pi}{\lambda}\lambda - \omega t\right) \\
             &= A \sin(2\pi - \omega t)
\end{align}
$$

Since the sine function is periodic with a period of $2\pi$, this simplifies to

$$
y(\lambda,t) = A \sin(-\omega t) = -A \sin(\omega t)
$$

## Final Result

The wavelength is

$$
\lambda = \frac{2\pi}{k}
$$

The phase velocity is

$$
v = \frac{\omega}{k}
$$

For the specific parameters, the velocity is

$$
v = 5\ \mathrm{m/s}
$$

Comparing $y(0,t)$ and $y(\lambda,t)$, we verify that they are identical. The point at $x = \lambda$ oscillates completely in phase with the point at $x = 0$.

## Interpretation

The wavelength $\lambda$ serves as the fundamental spatial period of the disturbance. The phase velocity reflects how quickly the entire shape of the wave moves along the axis. Because $x=0$ and $x=\lambda$ are separated by exactly one wavelength, their transverse motions are identical at all times $t$, confirming the spatial periodicity of the wave.
# Task 04 – Wave equation

## Problem Statement

The function is given by

$$
y(x,t) = A \cos(kx - \omega t)
$$

Verify that it satisfies the wave equation

$$
\frac{\partial^2 y}{\partial t^2} = v^2 \frac{\partial^2 y}{\partial x^2}
$$

and determine the relationship between $v$, $k$, and $\omega$.

## Theory

The one-dimensional linear wave equation describes the propagation of non-dispersive waves through a medium. For a mathematical function to represent a valid traveling wave in such a system, its second partial derivative with respect to time must be directly proportional to its second partial derivative with respect to space. The constant of proportionality is the square of the phase velocity, $v^2$.

## Step-by-Step Solution

First, the partial derivatives of the function $y(x,t)$ with respect to the spatial coordinate $x$ are calculated. The first spatial derivative is

$$
\frac{\partial y}{\partial x} = -A k \sin(kx - \omega t)
$$

Differentiating a second time yields the second spatial derivative:

$$
\frac{\partial^2 y}{\partial x^2} = -A k^2 \cos(kx - \omega t)
$$

Next, the partial derivatives of $y(x,t)$ with respect to time $t$ are calculated. The first temporal derivative is

$$
\frac{\partial y}{\partial t} = A \omega \sin(kx - \omega t)
$$

Differentiating a second time yields the second temporal derivative:

$$
\frac{\partial^2 y}{\partial t^2} = -A \omega^2 \cos(kx - \omega t)
$$

Now, both second derivatives are substituted into the given wave equation:

$$
-A \omega^2 \cos(kx - \omega t) = v^2 \left[ -A k^2 \cos(kx - \omega t) \right]
$$

Assuming the amplitude $A$ is non-zero and evaluating at points where the cosine term is not identically zero, the common factor $-A \cos(kx - \omega t)$ can be divided out from both sides. This leaves

$$
\omega^2 = v^2 k^2
$$

Taking the principal square root of both sides to solve for the phase velocity $v$ yields

$$
v = \frac{\omega}{k}
$$

## Final Result

The substitution into the differential equation confirms that the function is a valid solution. The algebraic relationship required for this to hold true is

$$
v = \frac{\omega}{k}
$$

## Interpretation

The formal substitution demonstrates that the geometric parameters of the harmonic wave (spatial wavenumber $k$ and angular frequency $\omega$) are fundamentally linked to the physical propagation speed $v$ of the medium. Because $v$ is established as a constant ratio of $\omega$ to $k$, the wave $y(x,t)$ propagates uniformly along the spatial axis without any alteration to its shape over time.
# Task 05 – Superposition of waves, beats, and group velocity

## Problem Statement

Two harmonic waves are given by

$$
y_1(x,t) = A\sin(kx-\omega t)
$$

$$
y_2(x,t) = A\sin(kx-(\omega+\Delta\omega)t)
$$

Determine the resultant wave $y = y_1 + y_2$ and express it in a product form (carrier × envelope). Identify the beat frequency and the beat period at the point $x=0$. Interpret the physical meaning of the envelope and the carrier wave.

## Theory

The principle of superposition dictates that the resultant displacement is the algebraic sum of individual wave displacements. When two waves of slightly different frequencies interfere, they produce a phenomenon known as beats. The macroscopic amplitude of the wave slowly modulates over time. The superposition is calculated using the trigonometric identity:

$$
\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)
$$

## Step-by-Step Solution

Let $\alpha = kx - \omega t$ and $\beta = kx - (\omega + \Delta\omega)t$. Adding $y_1$ and $y_2$ yields

$$
y(x,t) = A[\sin(kx-\omega t) + \sin(kx-\omega t - \Delta\omega t)]
$$

Applying the sum-to-product identity:

$$
\frac{\alpha + \beta}{2} = \frac{2kx - 2\omega t - \Delta\omega t}{2} = kx - \left(\omega + \frac{\Delta\omega}{2}\right)t
$$

$$
\frac{\alpha - \beta}{2} = \frac{\Delta\omega t}{2}
$$

The superposition equation becomes

$$
y(x,t) = 2A \cos\left(\frac{\Delta\omega}{2}t\right) \sin\left(kx - \left(\omega + \frac{\Delta\omega}{2}\right)t\right)
$$

At the point $x = 0$, the resultant wave is evaluated as

$$
y(0,t) = 2A \cos\left(\frac{\Delta\omega}{2}t\right) \sin\left(-\left(\omega + \frac{\Delta\omega}{2}\right)t\right)
$$

The amplitude modulation relies on the absolute value of the cosine term. Because the magnitude of a cosine wave peaks twice per full cycle, the envelope varies at an angular frequency of $\Delta\omega$.

The beat angular frequency is

$$
\omega_{\text{beat}} = \Delta\omega
$$

The beat frequency $f_{\text{beat}}$ and period $T_{\text{beat}}$ are

$$
f_{\text{beat}} = \frac{\Delta\omega}{2\pi}
$$

$$
T_{\text{beat}} = \frac{1}{f_{\text{beat}}} = \frac{2\pi}{\Delta\omega}
$$

## Final Result

The resultant wave function is

$$
y(x,t) = \left[ 2A \cos\left(\frac{\Delta\omega}{2}t\right) \right] \sin\left(kx - \left(\omega + \frac{\Delta\omega}{2}\right)t\right)
$$

The beat frequency and period at $x=0$ are

$$
f_{\text{beat}} = \frac{\Delta\omega}{2\pi}
$$

$$
T_{\text{beat}} = \frac{2\pi}{\Delta\omega}
$$

## Interpretation

The cosine term in the brackets describes the **envelope**, which represents the slowly varying amplitude that modulates the wave. The sine term represents the **carrier wave**, which oscillates rapidly at the average angular frequency. The envelope moves at the group velocity, carrying the energy of the wave packet, while the individual ripples of the carrier wave move at the phase velocity.
# Task 06 – Damped oscillator

## Problem Statement

The equation of motion for a damped oscillator is given by

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

Derive the general solution for the underdamped, critically damped, and overdamped cases. Explain how to prepare the equation for numerical integration using the RK4 method to investigate the effect of parameter $b$.

## Theory

A damped harmonic oscillator experiences a linear restoring force and a drag force proportional to its velocity. The system's dynamical behavior is governed by the roots of its characteristic equation. These roots define whether the system undergoes decaying oscillations, returns to equilibrium immediately without crossing it, or decays slowly.

## Step-by-Step Solution

Dividing the equation of motion by the mass $m$ yields

$$
\frac{d^2 x}{dt^2} + \frac{b}{m} \frac{dx}{dt} + \frac{k}{m} x = 0
$$

Introducing the damping coefficient $\gamma = b / (2m)$ and the natural angular frequency squared $\omega_0^2 = k / m$, the equation becomes

$$
\frac{d^2 x}{dt^2} + 2\gamma \frac{dx}{dt} + \omega_0^2 x = 0
$$

Assuming a solution of the form $x(t) = e^{rt}$, we obtain the characteristic equation

$$
r^2 + 2\gamma r + \omega_0^2 = 0
$$

The roots are derived via the quadratic formula:

$$
r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

The classification relies on the discriminant $\gamma^2 - \omega_0^2$.

**Case 1: Underdamped ($\gamma < \omega_0$)**

The discriminant is negative, leading to complex conjugate roots $r = -\gamma \pm i\omega_d$, where the damped angular frequency is

$$
\omega_d = \sqrt{\omega_0^2 - \gamma^2}
$$

The general solution is a decaying oscillation:

$$
x(t) = e^{-\gamma t} (C_1 \cos(\omega_d t) + C_2 \sin(\omega_d t))
$$

**Case 2: Critically Damped ($\gamma = \omega_0$)**

The root is real and repeated: $r = -\gamma$. The general solution requires a linearly independent term $t e^{-\gamma t}$:

$$
x(t) = (C_1 + C_2 t) e^{-\gamma t}
$$

**Case 3: Overdamped ($\gamma > \omega_0$)**

The roots are real and distinct.

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

For numerical analysis (such as the 4th-order Runge-Kutta method), the second-order differential equation must be reduced to a system of two coupled first-order equations. Let $v = dx/dt$:

$$
\begin{align}
\frac{dx}{dt} &= v \\
\frac{dv}{dt} &= -\frac{b}{m} v - \frac{k}{m} x
\end{align}
$$

These first-order equations can be evaluated iteratively to generate $x(t)$ and the phase portrait $v(x)$.

## Final Result

The general solutions are defined as follows:

Underdamped:

$$
x(t) = e^{-\frac{b}{2m} t} \left( C_1 \cos(\omega_d t) + C_2 \sin(\omega_d t) \right)
$$

Critically Damped:

$$
x(t) = (C_1 + C_2 t) e^{-\frac{b}{2m} t}
$$

Overdamped:

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

## Interpretation

The parameter $b$ acts as the control variable for energy dissipation. For small $b$, the system is underdamped and oscillates with a gradually decreasing amplitude. As $b$ reaches the critical threshold $2\sqrt{mk}$, the system becomes critically damped and returns to equilibrium in the minimum possible time without oscillating. If $b$ exceeds this threshold, the strong drag creates an overdamped state, resulting in a sluggish exponential decay toward equilibrium.

# Task 07 – Forced oscillator and resonance

## Problem Statement

The equation of motion for a forced oscillator is

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = F_0 \cos(\Omega t)
$$

Solve the equation analytically to determine the amplitude of steady-state oscillations as a function of $\Omega$. Discuss the numerical approach to investigating the steady-state amplitude and phase shift.

## Theory

A forced damped harmonic oscillator is driven by an external periodic force. The complete solution is the sum of a transient homogeneous solution (which decays due to damping) and a steady-state particular solution. The steady-state response oscillates at the driving frequency $\Omega$, but with an amplitude and phase shift that depend on the relationship between $\Omega$ and the natural frequency $\omega_0$.

## Step-by-Step Solution

We seek a steady-state particular solution of the form

$$
x_p(t) = A \cos(\Omega t - \delta)
$$

The first and second time derivatives are

$$
\frac{dx_p}{dt} = -A\Omega \sin(\Omega t - \delta)
$$

$$
\frac{d^2 x_p}{dt^2} = -A\Omega^2 \cos(\Omega t - \delta)
$$

Substituting these into the original differential equation yields

$$
-m A \Omega^2 \cos(\Omega t - \delta) - b A \Omega \sin(\Omega t - \delta) + k A \cos(\Omega t - \delta) = F_0 \cos(\Omega t)
$$

To simplify the algebra, we utilize the complex exponential method. We define a complex coordinate $z(t) = A e^{i(\Omega t - \delta)}$ such that $x_p(t) = \text{Re}[z(t)]$, and rewrite the driving force as $F_0 e^{i\Omega t}$:

$$
(-m \Omega^2 + i b \Omega + k) A e^{i(\Omega t - \delta)} = F_0 e^{i\Omega t}
$$

Dividing both sides by $e^{i(\Omega t - \delta)}$ leaves

$$
A (-m \Omega^2 + k + i b \Omega) = F_0 e^{i\delta}
$$

Expanding the right side into real and imaginary components:

$$
A (k - m \Omega^2) + i A b \Omega = F_0 \cos\delta + i F_0 \sin\delta
$$

Equating the magnitudes of both sides provides the steady-state amplitude $A$:

$$
A \sqrt{(k - m\Omega^2)^2 + (b\Omega)^2} = F_0
$$

$$
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
$$

Equating the ratio of the imaginary part to the real part provides the phase shift $\delta$:

$$
\tan\delta = \frac{b\Omega}{k - m\Omega^2}
$$

To analyze this system numerically, the resonance curve is constructed by iterating through an array of $\Omega$ values, computing $A(\Omega)$ and $\delta(\Omega)$ algebraically, and plotting the results to observe the peak amplitude and the phase transition.

## Final Result

The steady-state amplitude as a function of the driving frequency is

$$
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
$$

The phase shift is

$$
\delta(\Omega) = \arctan\left(\frac{b\Omega}{k - m\Omega^2}\right)
$$

## Interpretation

Resonance is the physical phenomenon where the oscillator responds with maximum amplitude. This peak occurs when the driving frequency $\Omega$ approaches the natural frequency $\omega_0 = \sqrt{k/m}$, minimizing the primary term in the denominator. The phase shift $\delta$ defines the lag between the driving force and the displacement. At very low frequencies, $\delta \approx 0$ (in phase). At resonance, $\delta = \pi/2$ (velocity is exactly in phase with the force, maximizing power transfer). At high frequencies, $\delta \to \pi$ (out of phase).
# Task 08 – Two coupled springs (two degrees of freedom)

## Problem Statement

Two masses are connected to rigid walls in a series configuration by springs with constants $k_1$, $k_2$, and $k_3$. Write the equations of motion, determine the natural frequencies and normal modes, and explain the mechanism of energy exchange.

## Theory

A system of two coupled masses possesses two degrees of freedom and therefore has two normal modes of oscillation. In a normal mode, all components of the system oscillate synchronously at the same natural frequency. Any arbitrary state of motion can be constructed as a linear superposition of these fundamental modes.

## Step-by-Step Solution

Let $x_1$ and $x_2$ denote the displacements of masses $m_1$ and $m_2$ from their equilibrium positions. The first spring $k_1$ connects the left wall to $m_1$. The middle spring $k_2$ connects $m_1$ to $m_2$. The third spring $k_3$ connects $m_2$ to the right wall.

By applying Newton's Second Law, the equations of motion are

$$
\begin{align}
m_1 \frac{d^2 x_1}{dt^2} &= -k_1 x_1 + k_2 (x_2 - x_1) \\
m_2 \frac{d^2 x_2}{dt^2} &= -k_2 (x_2 - x_1) - k_3 x_2
\end{align}
$$

This system is expressed as a matrix differential equation:

$$
M \frac{d^2 \mathbf{x}}{dt^2} = -K \mathbf{x}
$$

where the mass matrix $M$ and the stiffness matrix $K$ are

$$
M =
\begin{pmatrix}
m_1 & 0 \\
0 & m_2
\end{pmatrix}
$$

$$
K =
\begin{pmatrix}
k_1 + k_2 & -k_2 \\
-k_2 & k_2 + k_3
\end{pmatrix}
$$

Assuming harmonic solutions of the form $\mathbf{x}(t) = \mathbf{A} \cos(\omega t)$, the system reduces to an eigenvalue problem:

$$
(K - \omega^2 M) \mathbf{A} = 0
$$

For a non-trivial solution to exist, the determinant of the coefficient matrix must be zero:

$$
\det(K - \omega^2 M) = 0
$$

To find explicit normal modes, we assume a symmetric system where $m_1 = m_2 = m$ and $k_1 = k_2 = k_3 = k$. The determinant equation becomes

$$
\det
\begin{pmatrix}
2k - m\omega^2 & -k \\
-k & 2k - m\omega^2
\end{pmatrix}
= 0
$$

Expanding the determinant yields

$$
(2k - m\omega^2)^2 - k^2 = 0
$$

Taking the square root of both sides gives $2k - m\omega^2 = \pm k$. Solving for $\omega^2$ produces two natural frequencies:

$$
\omega_1^2 = \frac{k}{m}
$$

$$
\omega_2^2 = \frac{3k}{m}
$$

Substituting $\omega_1$ into the eigenvalue equation provides the first normal mode $\mathbf{A}_1$, where $x_1 = x_2$. Substituting $\omega_2$ provides the second normal mode $\mathbf{A}_2$, where $x_1 = -x_2$.

## Final Result

The generalized matrix equation of motion is

$$
\begin{pmatrix}
m_1 & 0 \\
0 & m_2
\end{pmatrix}
\frac{d^2}{dt^2}
\begin{pmatrix}
x_1 \\
x_2
\end{pmatrix}
=
-
\begin{pmatrix}
k_1 + k_2 & -k_2 \\
-k_2 & k_2 + k_3
\end{pmatrix}
\begin{pmatrix}
x_1 \\
x_2
\end{pmatrix}
$$

For the symmetric case ($m_1=m_2=m, k_1=k_2=k_3=k$), the natural frequencies are

$$
\omega_1 = \sqrt{\frac{k}{m}}, \quad \omega_2 = \sqrt{\frac{3k}{m}}
$$

## Interpretation

The two fundamental modes correspond to physical symmetries. The lower frequency mode ($\omega_1$) represents symmetric, in-phase motion where the masses move together and the central spring $k_2$ is neither compressed nor extended. The higher frequency mode ($\omega_2$) represents antisymmetric, out-of-phase motion where the masses move in opposite directions, forcing the central spring to undergo maximum deformation. When initial conditions do not purely match one mode (e.g., displacing only $m_1$), the resulting motion is a superposition of both modes. The slight difference in frequencies causes a beat phenomenon, manifested as a continuous, periodic exchange of kinetic energy between the two masses.
# Task 09 – Chain of $N$ springs (discrete wave model)

## Problem Statement

A system consists of $N$ masses connected by springs in a chain. Write down the equations of motion for the elements. Detail how a local initial disturbance propagates and evaluate the theoretical effect of the constants $k$ and $m$ on the propagation speed.

## Theory

A discrete chain of coupled masses and springs serves as a foundational model for acoustic waves in a crystal lattice or transverse waves on a loaded string. For low frequencies and long wavelengths (relative to the inter-mass spacing), the discrete equations converge to the continuous one-dimensional wave equation. 

## Step-by-Step Solution

Let the internal masses be $m$ and the spring constants be $k$. Let $x_i$ represent the displacement of the $i$-th mass from its equilibrium position. 

The net force acting on the $i$-th mass is strictly a consequence of its interactions with its immediate neighbors, $i-1$ and $i+1$. According to Hooke's law, the restoring force from the right spring is $k(x_{i+1} - x_i)$, and the restoring force from the left spring is $-k(x_i - x_{i-1})$.

Using Newton's Second Law, the equation of motion for the $i$-th mass is

$$
m \frac{d^2 x_i}{dt^2} = k(x_{i+1} - x_i) - k(x_i - x_{i-1})
$$

Factoring out the spring constant simplifies the expression to

$$
\frac{d^2 x_i}{dt^2} = \frac{k}{m} (x_{i+1} - 2x_i + x_{i-1})
$$

To solve the system numerically for $N$ masses (e.g., $N=20, 50, 100$), the set of $N$ second-order differential equations is mapped into a state vector of size $2N$ (positions and velocities). Boundary conditions must be set (e.g., fixed ends where $x_0 = 0$ and $x_{N+1} = 0$). By applying an initial Gaussian displacement to a few localized masses while setting all initial velocities to zero, numerical integration demonstrates a pulse splitting and traveling outward.

The term $(x_{i+1} - 2x_i + x_{i-1})$ represents the discrete spatial second derivative. By comparing this to the continuous wave equation $\partial^2 y / \partial t^2 = v^2 \partial^2 y / \partial x^2$, the propagation speed $v$ is shown to be proportional to $\sqrt{k/m}$.

## Final Result

The governing equation of motion for an internal mass $i$ is

$$
\frac{d^2 x_i}{dt^2} = \frac{k}{m} (x_{i+1} - 2x_i + x_{i-1})
$$

The theoretical wave propagation speed scales according to the relation

$$
v \propto \sqrt{\frac{k}{m}}
$$

## Interpretation

The initial local displacement establishes a tension gradient. This gradient acts as a restoring force that accelerates adjacent masses, resulting in the spatial translation of the disturbance along the chain. Increasing the spring stiffness $k$ raises the tension gradient for a given displacement, yielding higher accelerations and faster wave propagation. Conversely, increasing the mass $m$ increases the system's inertia, decreasing the acceleration of individual elements and thereby slowing the propagation speed.
# Task 10 – Double pendulum and deterministic chaos

## Problem Statement

Consider a double pendulum consisting of two massive points $m_1, m_2$ on massless rods $l_1, l_2$ in a uniform gravitational field $g$. Express the Cartesian coordinates as functions of the angles. Outline the numerical approach to investigating sensitivity to initial conditions by simulating an ensemble of 50 simultaneous trajectories to observe deterministic chaos.

## Theory

The double pendulum is a paradigm of deterministic chaos in classical mechanics. Despite being governed by exact, deterministic nonlinear differential equations derived from Lagrangian mechanics, the system exhibits extreme sensitivity to initial conditions. Trajectories in phase space that begin infinitesimally close to one another will ultimately diverge exponentially, rendering long-term predictions physically impossible.

## Step-by-Step Solution

The configuration is strictly defined by the generalized coordinates $\theta_1$ and $\theta_2$, representing the angles the upper and lower rods make with the vertical downward axis. 

The Cartesian coordinates for the first mass $m_1$, fixed at a distance $l_1$ from the origin, are determined via standard trigonometry:

$$
\begin{align}
x_1 &= l_1 \sin\theta_1 \\
y_1 &= -l_1 \cos\theta_1
\end{align}
$$

The coordinates for the second mass $m_2$ depend on the position of the first mass and the orientation of the second rod $l_2$:

$$
\begin{align}
x_2 &= x_1 + l_2 \sin\theta_2 \\
y_2 &= y_1 - l_2 \cos\theta_2
\end{align}
$$

Substituting $x_1$ and $y_1$ gives the complete absolute coordinates for $m_2$:

$$
\begin{align}
x_2 &= l_1 \sin\theta_1 + l_2 \sin\theta_2 \\
y_2 &= -l_1 \cos\theta_1 - l_2 \cos\theta_2
\end{align}
$$

To investigate deterministic chaos numerically, the second-order nonlinear differential equations for $\theta_1$ and $\theta_2$ are reduced to a system of four first-order ODEs. Using an integration scheme like RK4, the numerical stability is verified by computing the total mechanical energy at each time step and ensuring the energy drift remains within an acceptable tolerance dictated by the step size $\Delta t$.

To demonstrate sensitivity, a base initial state is chosen (e.g., $\theta_1 = \pi/2$, $\theta_2 = \pi/2$ with zero initial velocities). An ensemble of 50 copies of the system is generated, where the initial condition of $\theta_2$ for each copy is perturbed by a random microscopic variation on the order of $10^{-4}$ rad. The ODE system is solved simultaneously for all 50 states over the same time span.

## Final Result

The transformation from generalized angular coordinates to Cartesian visualization coordinates is given by:

$$
\begin{align}
x_1 &= l_1 \sin\theta_1 \\
y_1 &= -l_1 \cos\theta_1
\end{align}
$$

$$
\begin{align}
x_2 &= l_1 \sin\theta_1 + l_2 \sin\theta_2 \\
y_2 &= -l_1 \cos\theta_1 - l_2 \cos\theta_2
\end{align}
$$

## Interpretation

During the initial phase of the numerical simulation, all 50 pendulums will trace nearly identical, overlapping paths, seemingly behaving as a single predictable system. However, due to the underlying chaotic attractor, the microscopic coordinate differences $\delta \theta_2 \approx 10^{-4}$ are subjected to exponential amplification. After a specific duration (the Lyapunov time), the trajectories violently separate. The single path shatters into 50 distinct, highly erratic, and non-repeating curves that rapidly span the entire accessible physical space, visually confirming the loss of predictability.