# Problem 6 – Curve Length and Numerical Integration

We are given the parametric curve

- x(t) = t
- y(t) = t^2
- t in [0, 1]

We solve the problem step by step.

---

## 1. Position vector

The position vector is

r(t) = (x(t), y(t)) = (t, t^2)

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

## 3. Magnitude of the velocity

The speed is the magnitude of the velocity vector:

|v(t)| = sqrt(1^2 + (2t)^2)

So,

|v(t)| = sqrt(1 + 4t^2)

---

## 4. Arc length as an integral

The arc length of a parametric curve from t = 0 to t = 1 is

s = ∫_0^1 |v(t)| dt

Substitute |v(t)|:

s = ∫_0^1 sqrt(1 + 4t^2) dt

So the arc length integral is

s = ∫_0^1 sqrt(1 + 4t^2) dt

---

## 5. Analytical calculation of the integral

We compute

s = ∫_0^1 sqrt(1 + 4t^2) dt

Use the substitution

u = 2t

Then

du = 2 dt
dt = du / 2

Also:

- when t = 0, u = 0
- when t = 1, u = 2

So the integral becomes

s = ∫_0^2 sqrt(1 + u^2) · (1/2) du

Therefore,

s = (1/2) ∫_0^2 sqrt(1 + u^2) du

Now use the standard formula

∫ sqrt(1 + u^2) du = (1/2)u sqrt(1 + u^2) + (1/2) ln(u + sqrt(1 + u^2)) + C

So,

s = (1/2) * [ (1/2)u sqrt(1 + u^2) + (1/2) ln(u + sqrt(1 + u^2)) ] from 0 to 2

Simplify the factor:

s = (1/4) [ u sqrt(1 + u^2) + ln(u + sqrt(1 + u^2)) ] from 0 to 2

Now evaluate at u = 2:

- sqrt(1 + 2^2) = sqrt(5)

So the upper value is

2sqrt(5) + ln(2 + sqrt(5))

Now evaluate at u = 0:

- sqrt(1 + 0^2) = 1
- ln(0 + 1) = ln(1) = 0

So the lower value is

0

Hence,

s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]

This is the exact value.

### Exact result

s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]

### Approximate value

sqrt(5) ≈ 2.2360679

2sqrt(5) ≈ 4.4721358

ln(2 + sqrt(5)) ≈ ln(4.2360679) ≈ 1.4436355

Add them:

4.4721358 + 1.4436355 = 5.9157713

Now divide by 4:

s ≈ 1.4789428

So,

s ≈ 1.47894

---

## 6. Trapezoidal rule

To approximate

s = ∫_0^1 sqrt(1 + 4t^2) dt

with the trapezoidal rule, divide [0, 1] into N equal parts.

### Step 1. Step size

h = (1 - 0) / N = 1/N

### Step 2. Grid points

t_i = i h, for i = 0, 1, 2, ..., N

### Step 3. Function

f(t) = sqrt(1 + 4t^2)

### Step 4. Trapezoidal approximation

s_N = h [ (1/2)f(t_0) + f(t_1) + f(t_2) + ... + f(t_{N-1}) + (1/2)f(t_N) ]

That is,

s_N = (1/N) [ (1/2)f(0) + Σ_{i=1}^{N-1} f(i/N) + (1/2)f(1) ]

---

## 7. Error

If the exact arc length is s, then the absolute error is

error(N) = |s_N - s|

As N increases, the trapezoidal approximation should converge to the exact value.

---

## 8. Final mathematical results

- r(t) = (t, t^2)
- v(t) = (1, 2t)
- |v(t)| = sqrt(1 + 4t^2)
- s = ∫_0^1 sqrt(1 + 4t^2) dt
- s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]
- s ≈ 1.47894

---

