# Problem 5 – Trajectory Curvature and Normal Acceleration

We consider the ellipse

- x(t) = a cos(t)
- y(t) = b sin(t)

We solve each part step by step.

---

## 1. Velocity vector and acceleration vector

The position vector is

r(t) = (a cos(t), b sin(t))

### Velocity vector

Differentiate each component with respect to t:

- d/dt[a cos(t)] = -a sin(t)
- d/dt[b sin(t)] = b cos(t)

So,

v(t) = (-a sin(t), b cos(t))

### Speed

The magnitude of the velocity is

|v(t)| = sqrt[(-a sin(t))^2 + (b cos(t))^2]

|v(t)| = sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

### Acceleration vector

Differentiate v(t):

- d/dt[-a sin(t)] = -a cos(t)
- d/dt[b cos(t)] = -b sin(t)

So,

a(t) = (-a cos(t), -b sin(t))

---

## 2. Unit tangent vector

By definition,

T_hat(t) = v(t) / |v(t)|

Substitute the expressions:

T_hat(t) = (-a sin(t), b cos(t)) / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

So,

T_hat(t) = \left( 
\frac{-a \sin(t)}{\sqrt{a^2 \sin^2(t) + b^2 \cos^2(t)}},
\frac{b \cos(t)}{\sqrt{a^2 \sin^2(t) + b^2 \cos^2(t)}}
\right)

---

## 3. Decompose the acceleration into tangential and normal components

We want

a(t) = a_t(t) + a_n(t)

where

- a_t is the tangential component
- a_n is the normal component

---

### 3.1 Tangential component magnitude

The tangential acceleration magnitude is

a_t = d|v|/dt

We already have

|v(t)| = sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

Let

f(t) = a^2 sin^2(t) + b^2 cos^2(t)

Then

|v(t)| = sqrt[f(t)]

Differentiate:

d|v|/dt = (1 / (2 sqrt[f(t)])) · f'(t)

Now compute f'(t):

f'(t) = a^2 · 2 sin(t) cos(t) + b^2 · 2 cos(t)(-sin(t))

f'(t) = 2a^2 sin(t) cos(t) - 2b^2 sin(t) cos(t)

f'(t) = 2(a^2 - b^2) sin(t) cos(t)

Therefore,

a_t(t) = \frac{(a^2 - b^2)\sin(t)\cos(t)}{\sqrt{a^2\sin^2(t) + b^2\cos^2(t)}}

This is the scalar tangential acceleration.

So the tangential vector is

a_t_vec(t) = a_t(t) T_hat(t)

---

### 3.2 Normal acceleration magnitude

The normal acceleration magnitude can be found from

a_n = sqrt(|a|^2 - a_t^2)

but for planar motion it is often easier to use

a_n = |v × a| / |v|

Since the motion is in the plane, we treat v and a as 3D vectors with zero z-component:

v(t) = (-a sin(t), b cos(t), 0)

a(t) = (-a cos(t), -b sin(t), 0)

Compute the cross product:

v(t) × a(t) =
| i      j      k |
| -a sin(t)   b cos(t)   0 |
| -a cos(t)  -b sin(t)   0 |

Only the k-component remains:

k[( -a sin(t))(-b sin(t)) - (b cos(t))(-a cos(t))]

= k[ab sin^2(t) + ab cos^2(t)]

= k[ab(sin^2(t) + cos^2(t))]

= k(ab)

So

v(t) × a(t) = (0, 0, ab)

and therefore

|v(t) × a(t)| = ab

Now divide by |v(t)|:

a_n(t) = ab / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

So the magnitude of the normal acceleration is

a_n(t) = \frac{ab}{\sqrt{a^2\sin^2(t) + b^2\cos^2(t)}}

---

### 3.3 Normal acceleration vector

The normal acceleration vector points in the normal direction, and its magnitude is the quantity above.

So in decomposition form,

a(t) = a_t(t) T_hat(t) + a_n(t) N_hat(t)

where N_hat(t) is the unit normal vector.

---

## 4. Radius of curvature at t = 0 using a_n = v^2 / R

We use

a_n = v^2 / R

So

R = v^2 / a_n

We evaluate everything at t = 0.

---

### 4.1 Velocity at t = 0

v(0) = (-a sin(0), b cos(0)) = (0, b)

So

|v(0)| = b

Therefore

v^2(0) = b^2

---

### 4.2 Normal acceleration at t = 0

From the formula

a_n(t) = ab / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

At t = 0:

- sin(0) = 0
- cos(0) = 1

So

a_n(0) = ab / sqrt[a^2 · 0 + b^2 · 1]

a_n(0) = ab / b

a_n(0) = a

---

### 4.3 Radius of curvature

Now use

R(0) = v^2(0) / a_n(0)

So

R(0) = b^2 / a

Thus, the radius of curvature at t = 0 is

R(0) = b^2 / a

---

## 5. Compare with the circle case a = b

If a = b = R0, the ellipse becomes a circle of radius R0.

Then the formula gives

R(0) = b^2 / a = R0^2 / R0 = R0

So the radius of curvature is exactly the radius of the circle, as expected.

Also, for a circle:

- speed is constant
- tangential acceleration is zero
- all acceleration is normal acceleration

This matches the standard result for uniform circular motion.

---

## 6. Physical interpretation

The acceleration can be split into two parts:

- **Tangential acceleration** changes the magnitude of the velocity, meaning it changes how fast the particle moves.
- **Normal acceleration** changes the direction of the velocity, meaning it bends the trajectory.

So:

- if a_t is large, the particle speeds up or slows down strongly
- if a_n is large, the particle turns more sharply

The normal acceleration is therefore directly related to curvature.

---

## 7. Conceptual questions

### Q1. Does a greater trajectory curvature imply a greater normal acceleration?

Yes, if the speed is fixed.

This follows from

a_n = v^2 / R

Curvature is larger when the radius of curvature R is smaller. So if v is unchanged and R decreases, then a_n increases.

Therefore:

- greater curvature
- smaller radius of curvature
- greater normal acceleration

So yes, greater curvature implies greater normal acceleration for the same speed.

---

### Q2. Where on the ellipse is the trajectory more "curved": at the end of the major or minor semi-axis?

We compare the vertices.

#### At t = 0

This is the point

(x, y) = (a, 0)

The radius of curvature is

R_major_end = b^2 / a

#### At t = pi/2

This is the point

(x, y) = (0, b)

Using symmetry or the same formula, the radius of curvature there is

R_minor_end = a^2 / b

Now suppose a > b, so the x-axis is the major semi-axis.

Then

b^2 / a < a^2 / b

So the radius of curvature is smaller at (a, 0).

Smaller radius means greater curvature.

Therefore, the ellipse is more curved at the ends of the **major semi-axis**.

---

### Q3. Why can normal acceleration be interpreted as the cause of the change in the direction of motion?

Velocity is a vector, so it has:

- magnitude
- direction

Tangential acceleration acts along the direction of motion, so it changes the magnitude of velocity.

Normal acceleration acts perpendicular to the velocity, so it does not primarily change the speed. Instead, it turns the velocity vector.

That is why normal acceleration is responsible for the change in direction of motion.

A simple example is circular motion:

- the speed may stay constant
- but the direction changes continuously

This is only possible because there is a normal acceleration pointing toward the center.

---

## Final Results

### Velocity and acceleration

- v(t) = (-a sin(t), b cos(t))
- a(t) = (-a cos(t), -b sin(t))

### Speed

- |v(t)| = sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

### Unit tangent vector

- T_hat(t) = (-a sin(t), b cos(t)) / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

### Tangential acceleration magnitude

- a_t(t) = ((a^2 - b^2) sin(t) cos(t)) / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

### Normal acceleration magnitude

- a_n(t) = ab / sqrt[a^2 sin^2(t) + b^2 cos^2(t)]

### Radius of curvature at t = 0

- R(0) = b^2 / a

### Circle case a = b = R0

- R(0) = R0

### Key interpretation

- larger curvature means smaller radius of curvature
- for fixed speed, larger curvature means larger normal acceleration
- the ellipse is more curved at the ends of the major semi-axis
- normal acceleration changes the direction of motion
