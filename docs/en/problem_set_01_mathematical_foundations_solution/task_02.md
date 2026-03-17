<img width="751" height="790" alt="image" src="https://github.com/user-attachments/assets/ca2b49bc-bc9a-4b82-bdc3-b3c6c6d17ebe" />
# Problem 2 – Parametric Trajectory, Velocity, and Acceleration

## Given

The trajectory is

**r**(t) = (t^2, sin(t), 5)

This means the coordinate functions are:

- x(t) = t^2
- y(t) = sin(t)
- z(t) = 5

---

## 1. Velocity vector

The velocity is the derivative of the position vector:

v(t) = dr/dt

Differentiate each component separately:

- d/dt(t^2) = 2t
- d/dt(sin(t)) = cos(t)
- d/dt(5) = 0

So,

v(t) = (2t, cos(t), 0)

---

## 2. Acceleration vector

The acceleration is the derivative of the velocity vector:

a(t) = d^2r/dt^2 = dv/dt

Differentiate each component of v(t) = (2t, cos(t), 0):

- d/dt(2t) = 2
- d/dt(cos(t)) = -sin(t)
- d/dt(0) = 0

So,

a(t) = (2, -sin(t), 0)

---

## 3. Calculate |v(1)|

First compute v(1):

v(1) = (2(1), cos(1), 0) = (2, cos(1), 0)

Now compute its magnitude:

|v(1)| = sqrt(2^2 + cos^2(1) + 0^2)

|v(1)| = sqrt(4 + cos^2(1))

Approximate value:

cos(1) ≈ 0.5403

cos^2(1) ≈ 0.2919

So,

|v(1)| ≈ sqrt(4.2919) ≈ 2.0717

Final result:

|v(1)| = sqrt(4 + cos^2(1)) ≈ 2.0717

---

## 4. Calculate v · a

We use

v(t) = (2t, cos(t), 0)

a(t) = (2, -sin(t), 0)

The dot product is

v(t) · a(t) = (2t)(2) + (cos(t))(-sin(t)) + (0)(0)

Now simplify:

v(t) · a(t) = 4t - sin(t)cos(t)

Final result:

v(t) · a(t) = 4t - sin(t)cos(t)

You can also write it as

v(t) · a(t) = 4t - (1/2)sin(2t)

because

sin(t)cos(t) = (1/2)sin(2t)

---

## 5. Calculate v × a

We compute the cross product using the determinant form:

v(t) × a(t) =

| i        j        k |
| 2t     cos(t)     0 |
|  2    -sin(t)     0 |

Now expand:

= i(cos(t)·0 - 0·(-sin(t)))
- j(2t·0 - 0·2)
+ k(2t·(-sin(t)) - cos(t)·2)

Simplify each term:

- i-component = 0
- j-component = 0
- k-component = -2t sin(t) - 2 cos(t)

So,

v(t) × a(t) = (0, 0, -2t sin(t) - 2cos(t))

Final result:

v(t) × a(t) = (0, 0, -2t sin(t) - 2cos(t))

You can factor out -2:

v(t) × a(t) = (0, 0, -2(t sin(t) + cos(t)))

---

## 6. Interpretation of the trajectory

Since z(t) = 5 is constant, the curve lies entirely in the horizontal plane

z = 5

The trajectory is therefore the planar curve

x = t^2, y = sin(t)

embedded in 3D space at height 5.

---

## 7. Graph

Place this image in the same folder as your Markdown file and use:

![Trajectory with velocity and acceleration vectors](problem2_trajectory_vectors.png)

Selected points shown on the graph:
- t = -2
- t = -1
- t = 0
- t = 1
- t = 2

At those points:
- the **velocity vectors** are tangent to the curve
- the **acceleration vectors** show how the velocity is changing

---

## Final Answers

- v(t) = (2t, cos(t), 0)
- a(t) = (2, -sin(t), 0)
- |v(1)| = sqrt(4 + cos^2(1)) ≈ 2.0717
- v(t) · a(t) = 4t - sin(t)cos(t)
- v(t) × a(t) = (0, 0, -2t sin(t) - 2cos(t))
