# Problem 7 – Work of a Force Along a Trajectory

We are given the force field

- F(x, y) = (y, 2x)

and the trajectory

- x = t
- y = t^2
- t in [0, 1]

We solve the problem step by step.

---

## 1. Position vector of the trajectory

The trajectory can be written as the position vector

r(t) = (x(t), y(t)) = (t, t^2),  t in [0, 1]

---

## 2. Velocity vector

The velocity vector is the derivative of the position vector:

v(t) = dr/dt

Differentiate each component:

- d/dt[t] = 1
- d/dt[t^2] = 2t

So,

v(t) = (1, 2t)

---

## 3. Force along the trajectory

The force field is

F(x, y) = (y, 2x)

Now substitute the trajectory:

- x(t) = t
- y(t) = t^2

Therefore,

F(r(t)) = F(t, t^2) = (t^2, 2t)

---

## 4. Work as a line integral

The work done by the force along the curve is

W = ∫_C F · dr

Using the parameter t, this becomes

W = ∫_0^1 F(r(t)) · r'(t) dt

Since

- F(r(t)) = (t^2, 2t)
- r'(t) = v(t) = (1, 2t)

we compute the dot product:

F(r(t)) · r'(t) = (t^2, 2t) · (1, 2t)

Now multiply componentwise and add:

F(r(t)) · r'(t) = t^2 · 1 + 2t · 2t

F(r(t)) · r'(t) = t^2 + 4t^2

F(r(t)) · r'(t) = 5t^2

So the work integral becomes

W = ∫_0^1 5t^2 dt

---

## 5. Analytical calculation of the work

Now integrate:

W = ∫_0^1 5t^2 dt

Take the constant 5 outside:

W = 5 ∫_0^1 t^2 dt

We know

∫ t^2 dt = t^3 / 3

So

W = 5 [t^3 / 3]_0^1

Evaluate at the endpoints:

W = 5 (1^3 / 3 - 0^3 / 3)

W = 5/3

So the analytical result is

W = 5/3

Approximate value:

W ≈ 1.6666667

---

## 6. Riemann sum form of the integral

We want to write

W = ∫_0^1 5t^2 dt

as a limit of a Riemann sum.

Divide the interval [0, 1] into N equal parts.

### Step 1. Width of each interval

Δt = 1/N

### Step 2. Sample points

Using right endpoints:

t_i = i/N,  for i = 1, 2, ..., N

### Step 3. Riemann sum

Then

W ≈ Σ_{i=1}^N 5(t_i)^2 Δt

Substitute t_i = i/N and Δt = 1/N:

W_N = Σ_{i=1}^N 5(i/N)^2 (1/N)

So

W_N = Σ_{i=1}^N 5i^2 / N^3

Thus the exact integral can be written as

W = lim_{N→∞} Σ_{i=1}^N 5(i/N)^2 (1/N)

or equivalently

W = lim_{N→∞} Σ_{i=1}^N 5i^2 / N^3

---

## 7. Final results

- r(t) = (t, t^2)
- v(t) = (1, 2t)
- F(r(t)) = (t^2, 2t)
- F(r(t)) · v(t) = 5t^2
- W = ∫_0^1 5t^2 dt
- W = 5/3 ≈ 1.6666667

---
