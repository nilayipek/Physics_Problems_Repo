# Problem 8 – First-Order Differential Equation

We are given the differential equation

dy/dt = -k y

We solve it step by step and then provide an HTML/JS application to visualize the solution for different values of the parameter k and different initial conditions y(0).

---

## 1. Type of equation

The equation

dy/dt = -k y

is a **first-order ordinary differential equation**.

It is also:

- **separable**
- **linear**
- **homogeneous**

The easiest method here is separation of variables.

---

## 2. Solve the equation by separation of variables

We start with

dy/dt = -k y

Assume y ≠ 0, and divide both sides by y:

(1/y) dy/dt = -k

Now write it in differential form:

(1/y) dy = -k dt

Now integrate both sides:

∫ (1/y) dy = ∫ -k dt

The integrals are:

ln|y| = -kt + C

where C is the integration constant.

---

## 3. Solve for y(t)

Exponentiate both sides:

e^(ln|y|) = e^(-kt + C)

So,

|y| = e^C e^(-kt)

Since e^C is just a positive constant, we rename it as C1:

|y| = C1 e^(-kt)

Allowing the constant to absorb the sign, we write the general solution as

y(t) = C e^(-kt)

where C is any real constant.

---

## 4. Use the initial condition y(0)

Let

y(0) = y0

Substitute t = 0 into the general solution:

y(0) = C e^0 = C

So,

C = y0

Therefore, the solution satisfying the initial condition y(0) = y0 is

y(t) = y0 e^(-kt)

---

## 5. Final solution

### General solution

y(t) = C e^(-kt)

### Solution with initial condition y(0) = y0

y(t) = y0 e^(-kt)

---

## 6. Interpretation of the solution

The behavior depends on the sign of k.

### Case 1: k > 0

y(t) = y0 e^(-kt)

The exponential factor decreases as t increases, so the solution decays toward 0.

This models **exponential decay**.

Examples:
- cooling
- radioactive decay
- discharge of a capacitor
- damping

---

### Case 2: k = 0

Then the equation becomes

dy/dt = 0

So y is constant:

y(t) = y0

---

### Case 3: k < 0

Then

y(t) = y0 e^(-kt) = y0 e^(|k|t)

which grows exponentially in magnitude.

This is **exponential growth**.

---

## 7. Check the solution

Take

y(t) = y0 e^(-kt)

Differentiate:

dy/dt = y0 (-k) e^(-kt)

So,

dy/dt = -k y0 e^(-kt)

But

y0 e^(-kt) = y(t)

therefore

dy/dt = -k y(t)

So the solution is correct.

---

## 8. Summary

- Differential equation: dy/dt = -k y
- General solution: y(t) = C e^(-kt)
- With y(0) = y0: y(t) = y0 e^(-kt)

---
