# Problem 4 – Geometry of Parametric Curves

We investigate each curve step by step.

For each one, we will:

1. Eliminate the parameter (if possible)
2. Determine the type of curve
3. Compute the velocity vector v(t)
4. Compute the acceleration vector a(t)
5. Check whether |v(t)| or |a(t)| is constant

---

# A) x(t) = R cos(t), y(t) = R sin(t)

## 1. Eliminate the parameter

We have

x = R cos(t)
y = R sin(t)

Divide by R:

x / R = cos(t)
y / R = sin(t)

Now use the identity

cos^2(t) + sin^2(t) = 1

So

(x / R)^2 + (y / R)^2 = 1

Therefore,

x^2 + y^2 = R^2

## 2. Type of curve

This is a **circle** centered at the origin with radius R.

## 3. Velocity vector

Differentiate each component:

x'(t) = d/dt [R cos(t)] = -R sin(t)
y'(t) = d/dt [R sin(t)] = R cos(t)

So

v(t) = (-R sin(t), R cos(t))

## 4. Acceleration vector

Differentiate the velocity components:

x''(t) = d/dt [-R sin(t)] = -R cos(t)
y''(t) = d/dt [R cos(t)] = -R sin(t)

So

a(t) = (-R cos(t), -R sin(t))

## 5. Magnitudes

### Speed

|v(t)| = sqrt((-R sin(t))^2 + (R cos(t))^2)

= sqrt(R^2 sin^2(t) + R^2 cos^2(t))

= sqrt(R^2 (sin^2(t) + cos^2(t)))

= sqrt(R^2)

= R

So the speed is constant:

|v(t)| = R

### Acceleration magnitude

|a(t)| = sqrt((-R cos(t))^2 + (-R sin(t))^2)

= sqrt(R^2 cos^2(t) + R^2 sin^2(t))

= sqrt(R^2 (cos^2(t) + sin^2(t)))

= R

So the acceleration magnitude is also constant:

|a(t)| = R

## Final conclusion for A

- Parameter eliminated: x^2 + y^2 = R^2
- Curve type: circle
- v(t) = (-R sin(t), R cos(t))
- a(t) = (-R cos(t), -R sin(t))
- |v(t)| = R = constant
- |a(t)| = R = constant

---

# B) x(t) = a cos(t), y(t) = b sin(t)

## 1. Eliminate the parameter

We have

x = a cos(t)
y = b sin(t)

Divide:

x / a = cos(t)
y / b = sin(t)

Use the identity

cos^2(t) + sin^2(t) = 1

So

(x / a)^2 + (y / b)^2 = 1

Therefore,

x^2 / a^2 + y^2 / b^2 = 1

## 2. Type of curve

This is an **ellipse** centered at the origin, with semi-axis a in the x-direction and semi-axis b in the y-direction.

## 3. Velocity vector

Differentiate:

x'(t) = -a sin(t)
y'(t) = b cos(t)

So

v(t) = (-a sin(t), b cos(t))

## 4. Acceleration vector

Differentiate again:

x''(t) = -a cos(t)
y''(t) = -b sin(t)

So

a(t) = (-a cos(t), -b sin(t))

## 5. Magnitudes

### Speed

|v(t)| = sqrt((-a sin(t))^2 + (b cos(t))^2)

= sqrt(a^2 sin^2(t) + b^2 cos^2(t))

This is generally **not constant**, unless a = b.

If a = b = R, then the ellipse becomes a circle and the speed is constant.

### Acceleration magnitude

|a(t)| = sqrt((-a cos(t))^2 + (-b sin(t))^2)

= sqrt(a^2 cos^2(t) + b^2 sin^2(t))

This is also generally **not constant**, unless a = b.

## Final conclusion for B

- Parameter eliminated: x^2 / a^2 + y^2 / b^2 = 1
- Curve type: ellipse
- v(t) = (-a sin(t), b cos(t))
- a(t) = (-a cos(t), -b sin(t))
- |v(t)| = sqrt(a^2 sin^2(t) + b^2 cos^2(t)) → not constant in general
- |a(t)| = sqrt(a^2 cos^2(t) + b^2 sin^2(t)) → not constant in general

---

# C) x(t) = t, y(t) = t^2

## 1. Eliminate the parameter

Since

x = t

we can substitute t = x into y:

y = t^2 = x^2

Therefore,

y = x^2

## 2. Type of curve

This is a **parabola** opening upward.

## 3. Velocity vector

Differentiate:

x'(t) = d/dt [t] = 1
y'(t) = d/dt [t^2] = 2t

So

v(t) = (1, 2t)

## 4. Acceleration vector

Differentiate again:

x''(t) = 0
y''(t) = 2

So

a(t) = (0, 2)

## 5. Magnitudes

### Speed

|v(t)| = sqrt(1^2 + (2t)^2)

= sqrt(1 + 4t^2)

This depends on t, so it is **not constant**.

### Acceleration magnitude

|a(t)| = sqrt(0^2 + 2^2) = 2

So the acceleration magnitude is constant:

|a(t)| = 2

## Final conclusion for C

- Parameter eliminated: y = x^2
- Curve type: parabola
- v(t) = (1, 2t)
- a(t) = (0, 2)
- |v(t)| = sqrt(1 + 4t^2) → not constant
- |a(t)| = 2 = constant

---

# D) x(t) = cosh(t), y(t) = sinh(t)

## 1. Eliminate the parameter

We have

x = cosh(t)
y = sinh(t)

Use the hyperbolic identity

cosh^2(t) - sinh^2(t) = 1

So

x^2 - y^2 = 1

## 2. Type of curve

This is a **hyperbola**.

More precisely, it is the right branch of the hyperbola x^2 - y^2 = 1, because

cosh(t) >= 1 for all t.

## 3. Velocity vector

Differentiate:

x'(t) = d/dt [cosh(t)] = sinh(t)
y'(t) = d/dt [sinh(t)] = cosh(t)

So

v(t) = (sinh(t), cosh(t))

## 4. Acceleration vector

Differentiate again:

x''(t) = cosh(t)
y''(t) = sinh(t)

So

a(t) = (cosh(t), sinh(t))

## 5. Magnitudes

### Speed

|v(t)| = sqrt((sinh(t))^2 + (cosh(t))^2)

We can leave it as

|v(t)| = sqrt(sinh^2(t) + cosh^2(t))

This depends on t, so it is **not constant**.

Using hyperbolic identities, you may also write

cosh^2(t) + sinh^2(t) = cosh(2t)

so

|v(t)| = sqrt(cosh(2t))

### Acceleration magnitude

|a(t)| = sqrt((cosh(t))^2 + (sinh(t))^2)

= sqrt(cosh^2(t) + sinh^2(t))

= sqrt(cosh(2t))

This also depends on t, so it is **not constant**.

## Final conclusion for D

- Parameter eliminated: x^2 - y^2 = 1
- Curve type: hyperbola (right branch)
- v(t) = (sinh(t), cosh(t))
- a(t) = (cosh(t), sinh(t))
- |v(t)| = sqrt(sinh^2(t) + cosh^2(t)) = sqrt(cosh(2t)) → not constant
- |a(t)| = sqrt(cosh^2(t) + sinh^2(t)) = sqrt(cosh(2t)) → not constant

---

# Final Summary

## A) Circle
- Equation: x^2 + y^2 = R^2
- v(t) = (-R sin(t), R cos(t))
- a(t) = (-R cos(t), -R sin(t))
- |v(t)| = R → constant
- |a(t)| = R → constant

## B) Ellipse
- Equation: x^2 / a^2 + y^2 / b^2 = 1
- v(t) = (-a sin(t), b cos(t))
- a(t) = (-a cos(t), -b sin(t))
- |v(t)| = sqrt(a^2 sin^2(t) + b^2 cos^2(t)) → not constant in general
- |a(t)| = sqrt(a^2 cos^2(t) + b^2 sin^2(t)) → not constant in general

## C) Parabola
- Equation: y = x^2
- v(t) = (1, 2t)
- a(t) = (0, 2)
- |v(t)| = sqrt(1 + 4t^2) → not constant
- |a(t)| = 2 → constant

## D) Hyperbola
- Equation: x^2 - y^2 = 1
- v(t) = (sinh(t), cosh(t))
- a(t) = (cosh(t), sinh(t))
- |v(t)| = sqrt(cosh(2t)) → not constant
- |a(t)| = sqrt(cosh(2t)) → not constant
