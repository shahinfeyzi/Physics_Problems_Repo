# Problem Set 01 – Mathematical Foundations

---

## Task 1 – Vectors and Linear Transformations

### Problem Statement
Given two vectors in three-dimensional space:

$$
\vec a = (2,-1,3), \qquad \vec b = (1,4,-2)
$$

* Calculate the lengths $|\vec a|$ and $|\vec b|$.
* Determine the normalized vector $\hat a$.
* Calculate the dot product $\vec a \cdot \vec b$ and the angle between the vectors.
* Calculate the cross product $\vec a \times \vec b$ and the area of the parallelogram spanned by them.
* For a given matrix $A$, calculate $A\vec a$, $\det A$, and check orientation preservation.

### Theory
The magnitude of a vector $\vec{v} = (x, y, z)$ is defined as:

$$
|\vec{v}| = \sqrt{x^2 + y^2 + z^2}
$$

The dot product relates to the angle $\theta$ via:

$$
\vec a \cdot \vec b = |\vec a||\vec b| \cos \theta
$$

The magnitude of the cross product $|\vec a \times \vec b|$ represents the area of the parallelogram formed by the two vectors. A transformation $A$ preserves orientation if $\det A > 0$.

### Step-by-Step Solution

**1. Vector Magnitudes**

$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2} = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2} = \sqrt{1 + 16 + 4} = \sqrt{21}
$$

**2. Normalization**

$$
\hat a = \frac{\vec a}{|\vec a|} = \frac{1}{\sqrt{14}}(2, -1, 3) = \left( \frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

**3. Dot Product and Angle**

$$
\vec a \cdot \vec b = (2)(1) + (-1)(4) + (3)(-2) = 2 - 4 - 6 = -8
$$

To find the angle $\theta$:

$$
\cos \theta = \frac{\vec a \cdot \vec b}{|\vec a||\vec b|} = \frac{-8}{\sqrt{14}\sqrt{21}} = \frac{-8}{\sqrt{294}} = \frac{-8}{7\sqrt{6}}
$$

$$
\theta = \arccos\left( \frac{-8}{7\sqrt{6}} \right)
$$

**4. Cross Product and Area**

$$
\vec a \times \vec b = \begin{pmatrix} \hat i & \hat j & \hat k \\ 2 & -1 & 3 \\ 1 & 4 & -2 \end{pmatrix}
$$

$$
\vec a \times \vec b = \hat i(2 - 12) - \hat j(-4 - 3) + \hat k(8 - (-1)) = (-10, 7, 9)
$$

The area $S$ is the magnitude of this vector:

$$
S = |\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2} = \sqrt{100 + 49 + 81} = \sqrt{230}
$$

**5. Matrix Operations**

Given:

$$
A = \begin{pmatrix} 2 & 1 & 0 \\ 0 & 1 & -1 \\ 1 & 0 & 1 \end{pmatrix}
$$

Matrix-vector multiplication $A\vec a$:

$$
A\vec a = \begin{pmatrix} 2 & 1 & 0 \\ 0 & 1 & -1 \\ 1 & 0 & 1 \end{pmatrix} \begin{pmatrix} 2 \\ -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 2(2) + 1(-1) + 0(3) \\ 0(2) + 1(-1) - 1(3) \\ 1(2) + 0(-1) + 1(3) \end{pmatrix} = \begin{pmatrix} 3 \\ -4 \\ 5 \end{pmatrix}
$$

Determinant $\det A$:

$$
\det A = 2(1(1) - 0(-1)) - 1(0(1) - 1(-1)) + 0(\dots)
$$

$$
\det A = 2(1) - 1(1) = 1
$$

### Final Result
* $|\vec a| = \sqrt{14}$, $|\vec b| = \sqrt{21}$
* $\vec a \cdot \vec b = -8$, $\theta \approx 117.8^\circ$
* $\vec a \times \vec b = (-10, 7, 9)$, Area $= \sqrt{230}$
* $A\vec a = (3, -4, 5)$, $\det A = 1$

### Interpretation
Since $\det A = 1 > 0$, the transformation is non-singular and **preserves the orientation** of the coordinate system (it does not perform a reflection).
## Task 2 – Parametric Trajectory, Velocity, and Acceleration

### Problem Statement
The parametric equation of a trajectory is given by:

$$
\vec r(t) = (t^2, \sin t, 5)
$$

* Determine the velocity $\vec v(t) = \frac{d\vec r}{dt}$.
* Determine the acceleration $\vec a(t) = \frac{d^2 \vec r}{dt^2}$.
* Calculate the magnitude of the velocity at $t = 1$, $|\vec v(1)|$.
* Calculate the dot product $\vec v \cdot \vec a$.
* Calculate the cross product $\vec v \times \vec a$.

### Theory
In kinematics, the velocity vector is the first derivative of the position vector with respect to time, representing the instantaneous rate of change of position. The acceleration vector is the second derivative, representing the rate of change of velocity.

The magnitude (speed) is given by:

$$
v = |\vec v| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

### Step-by-Step Solution

**1. Velocity Vector**
Differentiating each component of $\vec r(t)$ with respect to $t$:

$$
\vec v(t) = \frac{d}{dt}(t^2, \sin t, 5) = (2t, \cos t, 0)
$$

**2. Acceleration Vector**
Differentiating the velocity vector with respect to $t$:

$$
\vec a(t) = \frac{d}{dt}(2t, \cos t, 0) = (2, -\sin t, 0)
$$

**3. Magnitude at $t = 1$**
First, evaluate $\vec v(1)$:

$$
\vec v(1) = (2(1), \cos(1), 0) = (2, \cos(1), 0)
$$

The magnitude is:

$$
|\vec v(1)| = \sqrt{2^2 + \cos^2(1) + 0^2} = \sqrt{4 + \cos^2(1)}
$$

Using the approximation $\cos(1) \approx 0.5403$:

$$
|\vec v(1)| \approx \sqrt{4 + 0.2919} \approx 2.0717
$$

**4. Dot Product $\vec v \cdot \vec a$**

$$
\vec v \cdot \vec a = (2t)(2) + (\cos t)(-\sin t) + (0)(0)
$$

$$
\vec v \cdot \vec a = 4t - \sin t \cos t = 4t - \frac{1}{2}\sin(2t)
$$

**5. Cross Product $\vec v \times \vec a$**

$$
\vec v \times \vec a = \begin{pmatrix} \hat i & \hat j & \hat k \\ 2t & \cos t & 0 \\ 2 & -\sin t & 0 \end{pmatrix}
$$

The $\hat i$ and $\hat j$ components are zero because the third column is zero:

$$
\vec v \times \vec a = \hat k \left[ (2t)(-\sin t) - (2)(\cos t) \right]
$$

$$
\vec v \times \vec a = (0, 0, -2t \sin t - 2 \cos t)
$$

### Final Result
* $\vec v(t) = (2t, \cos t, 0)$
* $\vec a(t) = (2, -\sin t, 0)$
* $|\vec v(1)| = \sqrt{4 + \cos^2(1)}$
* $\vec v \cdot \vec a = 4t - \sin t \cos t$
* $\vec v \times \vec a = (0, 0, -2t \sin t - 2 \cos t)$

### Interpretation
The trajectory lies entirely in the plane $z = 5$, as the $z$-component of velocity and acceleration is always zero. The cross product $\vec v \times \vec a$ points exclusively along the $z$-axis, which is consistent with planar motion in $xy$. Because $\vec v \cdot \vec a \neq 0$, the particle is changing both its direction and its speed simultaneously.
## Task 2 – Parametric Trajectory, Velocity, and Acceleration

### Problem Statement
The parametric equation of a trajectory is given by:

$$
\vec r(t) = (t^2, \sin t, 5)
$$

* Determine the velocity $\vec v(t) = \frac{d\vec r}{dt}$.
* Determine the acceleration $\vec a(t) = \frac{d^2 \vec r}{dt^2}$.
* Calculate the magnitude of the velocity at $t = 1$, $|\vec v(1)|$.
* Calculate the dot product $\vec v \cdot \vec a$.
* Calculate the cross product $\vec v \times \vec a$.

### Theory
In kinematics, the velocity vector is the first derivative of the position vector with respect to time, representing the instantaneous rate of change of position. The acceleration vector is the second derivative, representing the rate of change of velocity.

The magnitude (speed) is given by:

$$
v = |\vec v| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

### Step-by-Step Solution

**1. Velocity Vector**
Differentiating each component of $\vec r(t)$ with respect to $t$:

$$
\vec v(t) = \frac{d}{dt}(t^2, \sin t, 5) = (2t, \cos t, 0)
$$

**2. Acceleration Vector**
Differentiating the velocity vector with respect to $t$:

$$
\vec a(t) = \frac{d}{dt}(2t, \cos t, 0) = (2, -\sin t, 0)
$$

**3. Magnitude at $t = 1$**
First, evaluate $\vec v(1)$:

$$
\vec v(1) = (2(1), \cos(1), 0) = (2, \cos(1), 0)
$$

The magnitude is:

$$
|\vec v(1)| = \sqrt{2^2 + \cos^2(1) + 0^2} = \sqrt{4 + \cos^2(1)}
$$

Using the approximation $\cos(1) \approx 0.5403$:

$$
|\vec v(1)| \approx \sqrt{4 + 0.2919} \approx 2.0717
$$

**4. Dot Product $\vec v \cdot \vec a$**

$$
\vec v \cdot \vec a = (2t)(2) + (\cos t)(-\sin t) + (0)(0)
$$

$$
\vec v \cdot \vec a = 4t - \sin t \cos t = 4t - \frac{1}{2}\sin(2t)
$$

**5. Cross Product $\vec v \times \vec a$**

$$
\vec v \times \vec a = \begin{pmatrix} \hat i & \hat j & \hat k \\ 2t & \cos t & 0 \\ 2 & -\sin t & 0 \end{pmatrix}
$$

The $\hat i$ and $\hat j$ components are zero because the third column is zero:

$$
\vec v \times \vec a = \hat k \left[ (2t)(-\sin t) - (2)(\cos t) \right]
$$

$$
\vec v \times \vec a = (0, 0, -2t \sin t - 2 \cos t)
$$

### Final Result
* $\vec v(t) = (2t, \cos t, 0)$
* $\vec a(t) = (2, -\sin t, 0)$
* $|\vec v(1)| = \sqrt{4 + \cos^2(1)}$
* $\vec v \cdot \vec a = 4t - \sin t \cos t$
* $\vec v \times \vec a = (0, 0, -2t \sin t - 2 \cos t)$

### Interpretation
The trajectory lies entirely in the plane $z = 5$, as the $z$-component of velocity and acceleration is always zero. The cross product $\vec v \times \vec a$ points exclusively along the $z$-axis, which is consistent with planar motion in $xy$. Because $\vec v \cdot \vec a \neq 0$, the particle is changing both its direction and its speed simultaneously.
## Task 3 – Integration of Motion

### Problem Statement

**Part A: For a given velocity:**
$$
\vec v(t) = (2t, 3, -e^{-t}), \qquad \vec r(0) = (0, 1, 2)
$$
1. Determine the position vector $\vec r(t)$.
2. Determine the acceleration vector $\vec a(t)$.

**Part B: For a given acceleration:**
$$
\vec a(t) = (4, -\sin t, 0), \qquad \vec v(0) = (1, 0, 2), \qquad \vec r(0) = (0, 0, 0)
$$
1. Determine the velocity vector $\vec v(t)$.
2. Determine the position vector $\vec r(t)$.

---

### Theory
The Fundamental Theorem of Calculus allows us to retrieve position from velocity and velocity from acceleration through integration:

$$
\vec r(t) = \vec r(0) + \int_0^t \vec v(\tau) \, d\tau
$$

$$
\vec v(t) = \vec v(0) + \int_0^t \vec a(\tau) \, d\tau
$$

Conversely, acceleration is the time-derivative of velocity:

$$
\vec a(t) = \frac{d\vec v}{dt}
$$

---

### Step-by-Step Solution

#### Part A: Velocity to Position and Acceleration

**1. Determine $\vec r(t)$**
We integrate each component of $\vec v(t) = (2t, 3, -e^{-t})$ from $0$ to $t$:

$$
\begin{align}
x(t) &= x(0) + \int_0^t 2\tau \, d\tau = 0 + [\tau^2]_0^t = t^2 \\
y(t) &= y(0) + \int_0^t 3 \, d\tau = 1 + [3\tau]_0^t = 3t + 1 \\
z(t) &= z(0) + \int_0^t -e^{-\tau} \, d\tau = 2 + [e^{-\tau}]_0^t = 2 + (e^{-t} - 1) = e^{-t} + 1
\end{align}
$$

Thus:
$$
\vec r(t) = (t^2, 3t + 1, e^{-t} + 1)
$$

**2. Determine $\vec a(t)$**
Differentiating $\vec v(t)$ with respect to time:
$$
\vec a(t) = \frac{d}{dt}(2t, 3, -e^{-t}) = (2, 0, e^{-t})
$$

---

#### Part B: Acceleration to Velocity and Position

**1. Determine $\vec v(t)$**
Integrate $\vec a(t) = (4, -\sin t, 0)$ with initial condition $\vec v(0) = (1, 0, 2)$:

$$
\begin{align}
v_x(t) &= 1 + \int_0^t 4 \, d\tau = 1 + 4t \\
v_y(t) &= 0 + \int_0^t -\sin \tau \, d\tau = [\cos \tau]_0^t = \cos t - 1 \\
v_z(t) &= 2 + \int_0^t 0 \, d\tau = 2
\end{align}
$$

Thus:
$$
\vec v(t) = (4t + 1, \cos t - 1, 2)
$$

**2. Determine $\vec r(t)$**
Integrate $\vec v(t)$ with initial condition $\vec r(0) = (0, 0, 0)$:

$$
\begin{align}
x(t) &= \int_0^t (4\tau + 1) \, d\tau = [2\tau^2 + \tau]_0^t = 2t^2 + t \\
y(t) &= \int_0^t (\cos \tau - 1) \, d\tau = [\sin \tau - \tau]_0^t = \sin t - t \\
z(t) &= \int_0^t 2 \, d\tau = 2t
\end{align}
$$

Thus:
$$
\vec r(t) = (2t^2 + t, \sin t - t, 2t)
$$

---

### Final Result
**Part A:**
* $\vec r(t) = (t^2, 3t + 1, e^{-t} + 1)$
* $\vec a(t) = (2, 0, e^{-t})$

**Part B:**
* $\vec v(t) = (4t + 1, \cos t - 1, 2)$
* $\vec r(t) = (2t^2 + t, \sin t - t, 2t)$

---

### Interpretation
In Part A, the acceleration in the $z$-direction decays exponentially, meaning the force acting in that direction is vanishing over time. In Part B, the constant $z$-velocity ($v_z = 2$) indicates zero net force in the $z$-direction, leading to a linear displacement $z(t) = 2t$.
## Task 4 – Geometry of Parametric Curves

### Problem Statement
Investigate the following curves:
A) $x(t) = R\cos t, \quad y(t) = R\sin t$
B) $x(t) = a\cos t, \quad y(t) = b\sin t$
C) $x(t) = t, \quad y(t) = t^2$
D) $x(t) = \cosh t, \quad y(t) = \sinh t$

For each:
1. Eliminate the parameter.
2. Determine the curve type.
3. Find velocity $\vec v(t)$ and acceleration $\vec a(t)$.
4. Check for constant magnitudes $|\vec v|$ or $|\vec a|$.

---

### Theory
To eliminate the parameter $t$, we use trigonometric or hyperbolic identities:
* $\cos^2 t + \sin^2 t = 1$
* $\cosh^2 t - \sinh^2 t = 1$

The magnitude of a vector $\vec u = (u_x, u_y)$ is $|\vec u| = \sqrt{u_x^2 + u_y^2}$.

---

### Step-by-Step Solution

#### Curve A: Circle
1. **Eliminate parameter:** $(\frac{x}{R})^2 + (\frac{y}{R})^2 = \cos^2 t + \sin^2 t = 1 \implies x^2 + y^2 = R^2$
2. **Type:** Circle with radius $R$.
3. **Kinematics:**
   $$\vec v(t) = (-R\sin t, R\cos t)$$
   $$\vec a(t) = (-R\cos t, -R\sin t)$$
4. **Magnitudes:**
   $$|\vec v| = \sqrt{R^2\sin^2 t + R^2\cos^2 t} = R \quad (\text{Constant})$$
   $$|\vec a| = \sqrt{R^2\cos^2 t + R^2\sin^2 t} = R \quad (\text{Constant})$$

#### Curve B: Ellipse
1. **Eliminate parameter:** $(\frac{x}{a})^2 + (\frac{y}{b})^2 = \cos^2 t + \sin^2 t = 1 \implies \frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$
2. **Type:** Ellipse with semi-axes $a$ and $b$.
3. **Kinematics:**
   $$\vec v(t) = (-a\sin t, b\cos t)$$
   $$\vec a(t) = (-a\cos t, -b\sin t)$$
4. **Magnitudes:**
   $$|\vec v| = \sqrt{a^2\sin^2 t + b^2\cos^2 t} \quad (\text{Not constant if } a \neq b)$$
   $$|\vec a| = \sqrt{a^2\cos^2 t + b^2\sin^2 t} \quad (\text{Not constant if } a \neq b)$$

#### Curve C: Parabola
1. **Eliminate parameter:**
   $t = x \implies y = x^2$
2. **Type:** Parabola.
3. **Kinematics:**
   $$\vec v(t) = (1, 2t)$$
   $$\vec a(t) = (0, 2)$$
4. **Magnitudes:**
   $$|\vec v| = \sqrt{1 + 4t^2} \quad (\text{Not constant})$$
   $$|\vec a| = \sqrt{0^2 + 2^2} = 2 \quad (\text{Constant})$$

#### Curve D: Hyperbola
1. **Eliminate parameter:**
   $x^2 - y^2 = \cosh^2 t - \sinh^2 t = 1$
2. **Type:** Right branch of a hyperbola ($x \geq 1$).
3. **Kinematics:**
   $$\vec v(t) = (\sinh t, \cosh t)$$
   $$\vec a(t) = (\cosh t, \sinh t)$$
4. **Magnitudes:**
   $$|\vec v| = \sqrt{\sinh^2 t + \cosh^2 t} = \sqrt{\cosh(2t)} \quad (\text{Not constant})$$
   $$|\vec a| = \sqrt{\cosh^2 t + \sinh^2 t} = \sqrt{\cosh(2t)} \quad (\text{Not constant})$$

---

### Final Result
| Curve | Equation | Type | $|\vec v| = \text{const}$ | $|\vec a| = \text{const}$ |
| :--- | :--- | :--- | :--- | :--- |
| A | $x^2 + y^2 = R^2$ | Circle | Yes | Yes |
| B | $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$ | Ellipse | No | No |
| C | $y = x^2$ | Parabola | No | Yes |
| D | $x^2 - y^2 = 1$ | Hyperbola | No | No |

### Interpretation
Uniform circular motion (Curve A) is the only case where both speed and the magnitude of acceleration remain constant. In the parabolic case (Curve C), the constant acceleration $(0, 2)$ represents a uniform force field, such as gravity near the Earth's surface.
## Task 5 – Trajectory Curvature and Normal Acceleration

### Problem Statement
For an ellipse defined by:

$$
x = a \cos t, \qquad y = b \sin t
$$

1. Determine the velocity vector $\vec v(t)$ and the acceleration vector $\vec a(t)$.
2. Determine the unit tangent vector $\hat T(t)$.
3. Decompose the acceleration into tangential $\vec a_t$ and normal $\vec a_n$ components.
4. Determine the radius of curvature $R$ at $t = 0$.
5. Compare the results with the case of a circle ($a = b$).

---

### Theory
The acceleration vector can be decomposed into two perpendicular components:
* **Tangential acceleration ($a_t$):** Changes the magnitude of velocity (speed).
* **Normal acceleration ($a_n$):** Changes the direction of velocity.

The relationship between speed $v$ and the radius of curvature $R$ is:

$$
a_n = \frac{v^2}{R}
$$

---

### Step-by-Step Solution

**1. Kinematic Vectors**
Deriving the position vector $\vec r(t) = (a \cos t, b \sin t)$:

$$
\vec v(t) = (-a \sin t, b \cos t)
$$

$$
\vec a(t) = (-a \cos t, -b \sin t)
$$

**2. Unit Tangent Vector**
The magnitude of velocity (speed) is $v(t) = \sqrt{a^2 \sin^2 t + b^2 \cos^2 t}$.

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|} = \frac{1}{\sqrt{a^2 \sin^2 t + b^2 \cos^2 t}} (-a \sin t, b \cos t)
$$

**3. Normal Acceleration Magnitude**
The magnitude of the normal acceleration can be found using the formula:

$$
a_n = \frac{|\vec v \times \vec a|}{|\vec v|}
$$

Calculating the cross product (in 2D, we treat $z=0$):
$\vec v \times \vec a = (-a \sin t)(-b \sin t) - (b \cos t)(-a \cos t) = ab \sin^2 t + ab \cos^2 t = ab$.

$$
a_n(t) = \frac{ab}{\sqrt{a^2 \sin^2 t + b^2 \cos^2 t}}
$$

**4. Radius of Curvature at $t = 0$**
At $t = 0$:
* $v(0) = \sqrt{a^2(0) + b^2(1)} = b$
* $a_n(0) = \frac{ab}{\sqrt{0 + b^2}} = \frac{ab}{b} = a$

Using $R = \frac{v^2}{a_n}$:

$$
R(0) = \frac{b^2}{a}
$$

**5. Comparison with Circle**
For a circle where $a = b = r$:

$$
R = \frac{r^2}{r} = r
$$

In a circle, the radius of curvature is constant and equal to the radius of the circle at every point.

---

### Final Result
* $\vec v(t) = (-a \sin t, b \cos t)$
* $\hat T(t) = \frac{(-a \sin t, b \cos t)}{\sqrt{a^2 \sin^2 t + b^2 \cos^2 t}}$
* $a_n(t) = \frac{ab}{\sqrt{a^2 \sin^2 t + b^2 \cos^2 t}}$
* At $t=0$, the radius of curvature is $R = \frac{b^2}{a}$.

---

### Physical Interpretation

* **Greater curvature vs. Normal acceleration:** Yes. Since $a_n = v^2/R$, a smaller radius of curvature $R$ (higher curvature) results in a larger normal acceleration for a given speed.
* **Where is the ellipse more "curved"?** At the end of the **major axis** (where the "turn" is tightest). If $a > b$, then $R = b^2/a$ is the minimum radius of curvature.
* **Direction of motion:** Normal acceleration is always perpendicular to the velocity. Since it has no component in the direction of motion, it cannot change the speed; it only pulls the velocity vector "sideways," forcing the object to follow a curved path.
## Task 6 – Curve Length and Numerical Integration

### Problem Statement
A parametric trajectory in 2D is defined by:

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0, 1]
$$

1. Determine the velocity vector $\vec v(t) = \frac{d\vec r}{dt}$.
2. Determine the magnitude of the velocity $|\vec v(t)|$.
3. Write the arc length $s$ of the trajectory as an integral.
4. Calculate this integral analytically or reduce it to a form suitable for numerical methods.

---

### Theory
The arc length $s$ of a curve traced by a position vector $\vec r(t)$ from $t = a$ to $t = b$ is the integral of the scalar speed over that time interval:

$$
s = \int_{a}^{b} |\vec v(t)| \, dt = \int_{a}^{b} \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} \, dt
$$

For numerical estimation, the **Trapezoidal Rule** approximates the definite integral by summing the areas of trapezoids formed under the curve $f(t) = |\vec v(t)|$:

$$
\int_{a}^{b} f(t) \, dt \approx \frac{\Delta t}{2} \left[ f(t_0) + 2f(t_1) + \dots + 2f(t_{n-1}) + f(t_n) \right]
$$

---

### Step-by-Step Solution

**1. Velocity Vector**
Given the position vector $\vec r(t) = (t, t^2)$, we differentiate with respect to $t$:

$$
\vec v(t) = \left( \frac{dx}{dt}, \frac{dy}{dt} \right) = (1, 2t)
$$

**2. Magnitude of Velocity (Speed)**
The magnitude is calculated using the Euclidean norm:

$$
|\vec v(t)| = \sqrt{(1)^2 + (2t)^2} = \sqrt{1 + 4t^2}
$$

**3. Arc Length Integral**
Substituting the speed into the arc length formula for the interval $t \in [0, 1]$:

$$
s = \int_{0}^{1} \sqrt{1 + 4t^2} \, dt
$$

**4. Analytical Evaluation**
This integral takes the form $\int \sqrt{1 + u^2} \, du$. Using the substitution $u = 2t$ (where $du = 2dt$):

$$
s = \frac{1}{2} \int \sqrt{1 + u^2} \, du
$$

The standard integral for this form is $\frac{1}{2} \left( u\sqrt{1+u^2} + \ln|u + \sqrt{1+u^2}| \right)$. Applying the limits for $u$ (from $0$ to $2$):

$$
s = \left[ \frac{1}{2} t \sqrt{1 + 4t^2} + \frac{1}{4} \ln(2t + \sqrt{1 + 4t^2}) \right]_{0}^{1}
$$

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4} \ln(2 + \sqrt{5}) \approx 1.4789
$$

---

### Final Result
* **Velocity:** $\vec v(t) = (1, 2t)$
* **Speed:** $|\vec v(t)| = \sqrt{1 + 4t^2}$
* **Arc Length Integral:** $s = \int_{0}^{1} \sqrt{1 + 4t^2} \, dt$
* **Analytical Value:** $s \approx 1.4789$

---

### Interpretation
The arc length represents the actual distance traveled along the parabolic path. Because the path is curved, the arc length ($s \approx 1.4789$) is naturally greater than the straight-line distance (displacement) between the start point $(0,0)$ and end point $(1,1)$, which is $\sqrt{2} \approx 1.4142$.
## Task 7 – Work of a Force Along a Trajectory

### Problem Statement
Given a force field $\vec F(x, y)$ and a trajectory $C$:

$$
\vec F(x, y) = (y, 2x)
$$

The trajectory is defined by:
$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0, 1]
$$

1. Determine the velocity vector $\vec v(t) = \frac{d\vec r}{dt}$.
2. Calculate the work done by the force $\vec F$ along the trajectory using the line integral:
   $$
   W = \int_C \vec F \cdot d\vec r
   $$
3. Express the integral in a form suitable for numerical evaluation.

---

### Theory
The work $W$ done by a force $\vec F$ moving an object along a curve $C$ is defined as the line integral of the force along the path. Using the parameter $t$, this is expressed as:

$$
W = \int_{t_1}^{t_2} \vec F(\vec r(t)) \cdot \vec v(t) \, dt
$$

Where $\vec v(t) = \frac{d\vec r}{dt}$ is the velocity vector and the dot product $\vec F \cdot \vec v$ represents the instantaneous power (rate of work) if $t$ is time.

---

### Step-by-Step Solution

**1. Velocity Vector**
From the parametric equations $x(t) = t$ and $y(t) = t^2$:

$$
\vec r(t) = (t, t^2) \implies \vec v(t) = \frac{d\vec r}{dt} = (1, 2t)
$$

**2. Expressing Force in terms of $t$**
Substitute the parametric components $x = t$ and $y = t^2$ into the force field $\vec F(x, y) = (y, 2x)$:

$$
\vec F(t) = (t^2, 2t)
$$

**3. The Dot Product $\vec F \cdot \vec v$**
Calculate the scalar product of the force and velocity vectors:

$$
\vec F \cdot \vec v = (t^2)(1) + (2t)(2t) = t^2 + 4t^2 = 5t^2
$$

**4. Analytical Integration**
Integrate the power over the interval $t \in [0, 1]$:

$$
W = \int_0^1 5t^2 \, dt
$$

$$
W = \left[ \frac{5}{3}t^3 \right]_0^1 = \frac{5}{3} - 0 = \frac{5}{3} \approx 1.6667
$$

---

### Final Result
* **Velocity:** $\vec v(t) = (1, 2t)$
* **Force along path:** $\vec F(t) = (t^2, 2t)$
* **Work:** $W = \frac{5}{3}$ J (assuming SI units)

---

### Interpretation
The work is positive, meaning the force field generally acts in the direction of motion, adding energy to the system. Since the force $\vec F = (y, 2x)$ has a curl ($\frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} = 2 - 1 = 1 \neq 0$), the field is non-conservative. This implies the work done depends on the specific path taken between $(0,0)$ and $(1,1)$, not just the endpoints.
## Task 8 – First-Order Differential Equation

### Problem Statement
Consider the first-order ordinary differential equation (ODE):

$$
\frac{dy}{dt} = -k y
$$

1. Solve the equation analytically.
2. Determine the specific solution for an initial condition $y(0) = y_0$.
3. Analyze the behavior of the solution for different values of the parameter $k$.

---

### Theory
This is a **separable differential equation**. It describes a system where the rate of change of a quantity is proportional to the quantity itself, but in the opposite direction (decay).

In physics, this appears in:
* **Radioactive decay:** $dN/dt = -\lambda N$
* **Newton's Law of Cooling:** $dT/dt = -k(T - T_{env})$
* **Air resistance (linear):** $dv/dt = -kv$

---

### Step-by-Step Solution

**1. Separation of Variables**
To solve for $y(t)$, we rearrange the equation to group all $y$ terms on one side and $t$ terms on the other:

$$
\frac{1}{y} \, dy = -k \, dt
$$

**2. Integration**
Integrate both sides of the equation:

$$
\int \frac{1}{y} \, dy = \int -k \, dt
$$

$$
\ln|y| = -kt + C
$$

Where $C$ is the constant of integration.

**3. Exponentiation**
To solve for $y$, we take the exponential of both sides:

$$
|y| = e^{-kt + C} = e^C \cdot e^{-kt}
$$

Let $A = \pm e^C$ be a new constant:

$$
y(t) = A e^{-kt}
$$

**4. Applying Initial Conditions**
Using the condition $y(0) = y_0$ at $t = 0$:

$$
y(0) = A e^{-k(0)} = A \cdot 1 = y_0
$$

Therefore, the particular solution is:

$$
y(t) = y_0 e^{-kt}
$$

---

### Final Result
* **General Solution:** $y(t) = A e^{-kt}$
* **Particular Solution:** $y(t) = y_0 e^{-kt}$

---

### Interpretation
The solution is an **exponential decay** function. 
* If **$k > 0$**, $y(t)$ approaches zero as $t \to \infty$. The larger the value of $k$, the faster the decay occurs.
* The "half-life" or "characteristic time" $\tau = 1/k$ defines the scale at which the quantity significantly drops.
* If **$k < 0$**, the solution would represent exponential growth ($y(t) = y_0 e^{|k|t}$).
## Task 9 – Harmonic Oscillator

### Problem Statement
The equation of motion for a simple harmonic oscillator is given by:

$$
\frac{d^2 x}{dt^2} + \omega^2 x = 0
$$

1. Find the general solution to the differential equation.
2. Solve for specific initial conditions $x(0) = x_0$ and $v(0) = \dot{x}(0) = v_0$.
3. Analyze the physical parameters of the motion.

---

### Theory
This is a **second-order linear homogeneous differential equation** with constant coefficients. In physics, it describes systems where a restoring force is proportional to the displacement (Hooke's Law):

$$
F = -kx \implies m\frac{d^2 x}{dt^2} = -kx
$$

By defining $\omega^2 = k/m$, we obtain the standard form. The parameter $\omega$ represents the **angular frequency** of the oscillation.

---

### Step-by-Step Solution

**1. Characteristic Equation**
We assume a solution of the form $x(t) = e^{rt}$. Substituting this into the ODE:

$$
r^2 e^{rt} + \omega^2 e^{rt} = 0 \implies r^2 + \omega^2 = 0
$$

The roots are purely imaginary:
$$
r = \pm i\omega
$$

**2. General Solution**
Using Euler's formula, the general solution can be written in terms of sines and cosines:

$$
x(t) = C_1 \cos(\omega t) + C_2 \sin(\omega t)
$$

Alternatively, it can be expressed using amplitude $A$ and phase $\phi$:
$$
x(t) = A \cos(\omega t + \phi)
$$

**3. Applying Initial Conditions**
To find $C_1$ and $C_2$, we use $x(0) = x_0$ and $\dot{x}(0) = v_0$.

First, find the velocity expression:
$$
v(t) = \dot{x}(t) = -C_1 \omega \sin(\omega t) + C_2 \omega \cos(\omega t)
$$

At $t = 0$:
$$
x(0) = C_1 \cos(0) + C_2 \sin(0) = C_1 = x_0
$$
$$
v(0) = -x_0 \omega \sin(0) + C_2 \omega \cos(0) = C_2 \omega = v_0 \implies C_2 = \frac{v_0}{\omega}
$$

The particular solution is:
$$
x(t) = x_0 \cos(\omega t) + \frac{v_0}{\omega} \sin(\omega t)
$$

---

### Final Result
* **General Solution:** $x(t) = C_1 \cos(\omega t) + C_2 \sin(\omega t)$
* **Particular Solution:** $x(t) = x_0 \cos(\omega t) + \frac{v_0}{\omega} \sin(\omega t)$
* **Velocity:** $v(t) = -x_0 \omega \sin(\omega t) + v_0 \cos(\omega t)$
* **Acceleration:** $a(t) = -\omega^2 x(t)$

---

### Interpretation
The motion is periodic and sinusoidal. The acceleration is always directed toward the equilibrium position ($x=0$) and is proportional to the displacement. 
* The **period** is $T = \frac{2\pi}{\omega}$.
* The **frequency** is $f = \frac{1}{T} = \frac{\omega}{2\pi}$.
* Energy oscillates between kinetic (maximum at $x=0$) and potential (maximum at $x = \pm A$).
## Task 10 – Angular Momentum in Circular Motion

### Problem Statement
Consider circular motion in the $xy$ plane:

$$
\vec r(t) = (R \cos(\omega t), R \sin(\omega t), 0)
$$

1. Determine the velocity $\vec v(t) = \dot{\vec r}(t)$.
2. Calculate the angular momentum $\vec L(t) = m \vec r(t) \times \vec v(t)$.
3. Show that $|\vec L| = mR^2\omega$ and that $\vec L$ is perpendicular to the plane of motion.
4. Verify the relationship $\vec \tau = \frac{d\vec L}{dt}$ for uniform circular motion.

---

### Theory
Angular momentum $\vec L$ characterizes the "quantity of rotation" an object has relative to a specific origin. It is defined as the cross product of the position vector and the linear momentum:

$$
\vec L = \vec r \times \vec p = m (\vec r \times \vec v)
$$

The torque $\vec \tau$ is the rotational analogue of force and is defined as:

$$
\vec \tau = \vec r \times \vec F = \frac{d\vec L}{dt}
$$

In uniform circular motion, the speed is constant, but the direction of velocity changes continuously due to a centripetal force.

---

### Step-by-Step Solution

**1. Velocity Vector**
Differentiating the position vector $\vec r(t)$ with respect to time:

$$
\vec v(t) = \frac{d}{dt} (R \cos(\omega t), R \sin(\omega t), 0) = (-R\omega \sin(\omega t), R\omega \cos(\omega t), 0)
$$

**2. Angular Momentum Calculation**
Using the cross product definition:

$$
\vec L = m \begin{pmatrix} \hat i & \hat j & \hat k \\ R \cos(\omega t) & R \sin(\omega t) & 0 \\ -R\omega \sin(\omega t) & R\omega \cos(\omega t) & 0 \end{pmatrix}
$$

The $\hat i$ and $\hat j$ components are zero. The $\hat k$ component is:

$$
L_z = m [ (R \cos(\omega t))(R\omega \cos(\omega t)) - (R \sin(\omega t))(-R\omega \sin(\omega t)) ]
$$

$$
L_z = m R^2 \omega (\cos^2(\omega t) + \sin^2(\omega t)) = m R^2 \omega
$$

Thus:
$$
\vec L = (0, 0, m R^2 \omega)
$$

**3. Magnitude and Orientation**
The magnitude is $|\vec L| = \sqrt{0^2 + 0^2 + (mR^2\omega)^2} = mR^2\omega$. 
Since the vector only has a $z$-component, it is strictly perpendicular to the $xy$ plane in which the motion occurs.

**4. Torque and Derivative of L**
For uniform circular motion, $|\vec L|$ is constant and its direction is fixed (along the $z$-axis). Therefore:

$$
\vec \tau = \frac{d\vec L}{dt} = \frac{d}{dt} (0, 0, mR^2\omega) = (0, 0, 0)
$$

This is consistent with the fact that the centripetal force $\vec F_c$ is always anti-parallel to the position vector $\vec r$. Since $\vec F_c \parallel \vec r$, their cross product (torque) is zero:

$$
\vec \tau = \vec r \times \vec F_c = 0
$$

---

### Final Result
* **Velocity:** $\vec v(t) = (-R\omega \sin(\omega t), R\omega \cos(\omega t), 0)$
* **Angular Momentum:** $\vec L = (0, 0, mR^2\omega)$
* **Torque:** $\vec \tau = (0, 0, 0)$

---

### Interpretation
The angular momentum vector follows the **right-hand rule**: if the fingers of the right hand curl in the direction of the particle's rotation, the thumb points in the direction of $\vec L$. Because the torque is zero, the angular momentum of the system is conserved (remains constant in both magnitude and direction).