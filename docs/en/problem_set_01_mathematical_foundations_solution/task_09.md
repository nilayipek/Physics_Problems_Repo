# Problem 9 – Harmonic Oscillator

We are given the differential equation

x''(t) + ω^2 x(t) = 0

We solve it step by step.

---

## 1. Find the general solution

This is a second-order linear homogeneous differential equation with constant coefficients.

We try a solution of the form

x(t) = e^(rt)

where r is a constant.

### Step 1: Compute derivatives

If

x(t) = e^(rt)

then

x'(t) = r e^(rt)

x''(t) = r^2 e^(rt)

### Step 2: Substitute into the differential equation

Substitute into

x''(t) + ω^2 x(t) = 0

to get

r^2 e^(rt) + ω^2 e^(rt) = 0

Factor out e^(rt):

e^(rt) (r^2 + ω^2) = 0

Since e^(rt) is never zero, we must have

r^2 + ω^2 = 0

### Step 3: Solve the characteristic equation

r^2 = -ω^2

so

r = ± iω

### Step 4: Write the real-valued general solution

For roots ±iω, the general real solution is

x(t) = C1 cos(ωt) + C2 sin(ωt)

So the general solution is

x(t) = C1 cos(ωt) + C2 sin(ωt)

---

## 2. Solve for the initial conditions

Since the problem statement says "solve for the given initial conditions" but does not show specific values, we solve for the standard initial conditions

x(0) = x0
x'(0) = v0

where

- x0 is the initial position
- v0 is the initial velocity

### Step 1: Start from the general solution

x(t) = C1 cos(ωt) + C2 sin(ωt)

Differentiate:

x'(t) = -C1 ω sin(ωt) + C2 ω cos(ωt)

---

### Step 2: Use x(0) = x0

Set t = 0:

x(0) = C1 cos(0) + C2 sin(0)

Since

cos(0) = 1
sin(0) = 0

we get

x(0) = C1

Therefore

C1 = x0

---

### Step 3: Use x'(0) = v0

Set t = 0 in x'(t):

x'(0) = -C1 ω sin(0) + C2 ω cos(0)

Since

sin(0) = 0
cos(0) = 1

we get

x'(0) = C2 ω

Therefore

C2 = v0 / ω

---

### Step 4: Substitute back

So the solution satisfying the initial conditions is

x(t) = x0 cos(ωt) + (v0 / ω) sin(ωt)

---

## 3. Find x'(t) and x''(t)

We need these for the visualization.

### Velocity

Differentiate x(t):

x'(t) = -ω x0 sin(ωt) + v0 cos(ωt)

### Acceleration

Differentiate again:

x''(t) = -ω^2 x0 cos(ωt) - ω v0 sin(ωt)

You can also use the differential equation directly:

x''(t) = -ω^2 x(t)

which gives the same result.

---

## 4. Final results

### General solution

x(t) = C1 cos(ωt) + C2 sin(ωt)

### Solution with initial conditions x(0) = x0, x'(0) = v0

x(t) = x0 cos(ωt) + (v0 / ω) sin(ωt)

### First derivative

x'(t) = -ω x0 sin(ωt) + v0 cos(ωt)

### Second derivative

x''(t) = -ω^2 x0 cos(ωt) - ω v0 sin(ωt)

or equivalently

x''(t) = -ω^2 x(t)

---

## 5. Physical interpretation

This equation describes simple harmonic motion.

- x(t) is the displacement
- x'(t) is the velocity
- x''(t) is the acceleration
- ω is the angular frequency

The acceleration is always proportional to -x(t), which means it always points toward the equilibrium position. That is why the motion oscillates.

---

## 6. Example

If

ω = 2
x(0) = 1
x'(0) = 0

then

x(t) = cos(2t)

x'(t) = -2 sin(2t)

x''(t) = -4 cos(2t)

---
