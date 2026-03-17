# Problem 3 – Integration of Motion

---

# A) Given velocity

## Given

v(t) = (2t, 3, -e^(-t))

r(0) = (0, 1, 2)

We need to determine:

- r(t) = r(0) + ∫ from 0 to t of v(τ) dτ
- a(t)

---

## 1. Determine r(t)

We use

r(t) = r(0) + ∫_0^t v(τ) dτ

Substitute the given velocity:

r(t) = (0, 1, 2) + ∫_0^t (2τ, 3, -e^(-τ)) dτ

Integrate component by component:

r(t) = (0, 1, 2) + (∫_0^t 2τ dτ, ∫_0^t 3 dτ, ∫_0^t -e^(-τ) dτ)

### First component

∫_0^t 2τ dτ = [τ^2]_0^t = t^2 - 0 = t^2

### Second component

∫_0^t 3 dτ = [3τ]_0^t = 3t - 0 = 3t

### Third component

∫_0^t -e^(-τ) dτ

We know that

∫ -e^(-τ) dτ = e^(-τ)

So

∫_0^t -e^(-τ) dτ = [e^(-τ)]_0^t = e^(-t) - e^0 = e^(-t) - 1

Now substitute back:

r(t) = (0, 1, 2) + (t^2, 3t, e^(-t) - 1)

Add componentwise:

r(t) = (t^2, 1 + 3t, 2 + e^(-t) - 1)

r(t) = (t^2, 1 + 3t, 1 + e^(-t))

### Final result for position

r(t) = (t^2, 1 + 3t, 1 + e^(-t))

---

## 2. Determine a(t)

Acceleration is the derivative of velocity:

a(t) = dv/dt

Given

v(t) = (2t, 3, -e^(-t))

Differentiate each component:

- d/dt(2t) = 2
- d/dt(3) = 0
- d/dt(-e^(-t)) = e^(-t)

So

a(t) = (2, 0, e^(-t))

### Final result for acceleration

a(t) = (2, 0, e^(-t))

---

# B) Given acceleration

## Given

a(t) = (4, -sin(t), 0)

v(0) = (1, 0, 2)

r(0) = (0, 0, 0)

We need to determine:

- v(t) = v(0) + ∫_0^t a(τ) dτ
- r(t) = ∫_0^t v(τ) dτ + r(0)

---

## 1. Determine v(t)

We use

v(t) = v(0) + ∫_0^t a(τ) dτ

Substitute the given data:

v(t) = (1, 0, 2) + ∫_0^t (4, -sin(τ), 0) dτ

Integrate component by component:

v(t) = (1, 0, 2) + (∫_0^t 4 dτ, ∫_0^t -sin(τ) dτ, ∫_0^t 0 dτ)

### First component

∫_0^t 4 dτ = [4τ]_0^t = 4t

### Second component

∫_0^t -sin(τ) dτ

We know

∫ -sin(τ) dτ = cos(τ)

So

∫_0^t -sin(τ) dτ = [cos(τ)]_0^t = cos(t) - cos(0) = cos(t) - 1

### Third component

∫_0^t 0 dτ = 0

Now substitute back:

v(t) = (1, 0, 2) + (4t, cos(t) - 1, 0)

Add componentwise:

v(t) = (1 + 4t, cos(t) - 1, 2)

### Final result for velocity

v(t) = (1 + 4t, cos(t) - 1, 2)

---

## 2. Determine r(t)

We use

r(t) = ∫_0^t v(τ) dτ + r(0)

Since r(0) = (0, 0, 0), this becomes

r(t) = ∫_0^t v(τ) dτ

Substitute v(τ):

r(t) = ∫_0^t (1 + 4τ, cos(τ) - 1, 2) dτ

Integrate component by component:

r(t) = (∫_0^t (1 + 4τ) dτ, ∫_0^t (cos(τ) - 1) dτ, ∫_0^t 2 dτ)

### First component

∫_0^t (1 + 4τ) dτ = ∫_0^t 1 dτ + ∫_0^t 4τ dτ

= [τ]_0^t + [2τ^2]_0^t

= t + 2t^2

### Second component

∫_0^t (cos(τ) - 1) dτ = ∫_0^t cos(τ) dτ - ∫_0^t 1 dτ

= [sin(τ)]_0^t - [τ]_0^t

= sin(t) - t

### Third component

∫_0^t 2 dτ = [2τ]_0^t = 2t

Now combine the components:

r(t) = (t + 2t^2, sin(t) - t, 2t)

### Final result for position

r(t) = (t + 2t^2, sin(t) - t, 2t)

---

# Final Answers

## A) Given velocity

- r(t) = (t^2, 1 + 3t, 1 + e^(-t))
- a(t) = (2, 0, e^(-t))

## B) Given acceleration

- v(t) = (1 + 4t, cos(t) - 1, 2)
- r(t) = (t + 2t^2, sin(t) - t, 2t)
