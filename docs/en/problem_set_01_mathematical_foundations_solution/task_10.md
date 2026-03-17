# Problem 10 – Angular Momentum in Circular Motion

We consider the motion

r(t) = (R cos(ωt), R sin(ωt), 0)

This is circular motion in the xy-plane with radius R and angular frequency ω.

We solve each part step by step.

---

## 1. Determine the velocity vector

The velocity is the derivative of the position vector:

v(t) = dr/dt

Differentiate each component:

- d/dt [R cos(ωt)] = -Rω sin(ωt)
- d/dt [R sin(ωt)] = Rω cos(ωt)
- d/dt [0] = 0

So,

v(t) = (-Rω sin(ωt), Rω cos(ωt), 0)

### Final result

v(t) = (-Rω sin(ωt), Rω cos(ωt), 0)

---

## 2. Calculate the angular momentum

The angular momentum with respect to the origin is

L(t) = m r(t) × v(t)

We substitute

r(t) = (R cos(ωt), R sin(ωt), 0)

v(t) = (-Rω sin(ωt), Rω cos(ωt), 0)

So,

L(t) = m
| i              j              k |
| R cos(ωt)      R sin(ωt)      0 |
| -Rω sin(ωt)    Rω cos(ωt)     0 |

Now compute the determinant.

---

### i-component

R sin(ωt) · 0 - 0 · Rω cos(ωt) = 0

### j-component

R cos(ωt) · 0 - 0 · (-Rω sin(ωt)) = 0

Since the j-term is subtracted in the determinant formula, it is still 0.

### k-component

R cos(ωt) · Rω cos(ωt) - R sin(ωt) · (-Rω sin(ωt))

= R^2 ω cos^2(ωt) + R^2 ω sin^2(ωt)

Factor out R^2 ω:

= R^2 ω [cos^2(ωt) + sin^2(ωt)]

Use the identity

cos^2(ωt) + sin^2(ωt) = 1

So the k-component is

R^2 ω

Therefore,

r(t) × v(t) = (0, 0, R^2 ω)

Now multiply by m:

L(t) = (0, 0, mR^2ω)

### Final result

L(t) = (0, 0, mR^2ω)

---

## 3. Show that |L| = mR^2ω is constant

We found

L(t) = (0, 0, mR^2ω)

Its magnitude is

|L(t)| = sqrt(0^2 + 0^2 + (mR^2ω)^2)

= mR^2ω

So

|L| = mR^2ω

This does not depend on time, so it is constant.

### Final result

|L| = mR^2ω = constant

---

## 4. Show that L is perpendicular to the plane of motion

The motion takes place in the xy-plane because

r(t) = (R cos(ωt), R sin(ωt), 0)

so z = 0 for all t.

But we found

L(t) = (0, 0, mR^2ω)

This vector points in the z-direction.

A vector in the z-direction is perpendicular to the xy-plane.

Therefore,

- the plane of motion is the xy-plane
- the angular momentum vector is perpendicular to that plane

---

## 5. Interpret the direction of L (right-hand rule)

The position vector rotates from the positive x-axis toward the positive y-axis as t increases.

That is a counterclockwise rotation when viewed from above the positive z-axis.

Using the right-hand rule:

- curl the fingers of your right hand in the direction of motion
- your thumb points in the direction of angular momentum

So the angular momentum points in the positive z-direction.

Therefore,

L points along +k

If the motion were clockwise instead, then L would point in the negative z-direction.

---

## 6. Optional: Add a constant centripetal force and calculate the torque

For uniform circular motion, the required centripetal force points toward the origin.

The acceleration is

a(t) = dv/dt

Differentiate the velocity:

v(t) = (-Rω sin(ωt), Rω cos(ωt), 0)

Then

a(t) = (-Rω^2 cos(ωt), -Rω^2 sin(ωt), 0)

This can be written as

a(t) = -ω^2 r(t)

So the force is

F(t) = m a(t) = -mω^2 r(t)

In components,

F(t) = (-mω^2 R cos(ωt), -mω^2 R sin(ωt), 0)

This is a centripetal force because it always points opposite to r(t), that is, toward the origin.

---

## 7. Calculate the torque

Torque is

τ(t) = r(t) × F(t)

Since

F(t) = -mω^2 r(t)

we have

τ(t) = r(t) × (-mω^2 r(t))

Factor out the constant:

τ(t) = -mω^2 [r(t) × r(t)]

But any vector crossed with itself is zero:

r(t) × r(t) = 0

Therefore,

τ(t) = 0

### Final result

τ(t) = (0, 0, 0)

---

## 8. Verify that τ = dL/dt

We found

L(t) = (0, 0, mR^2ω)

This is constant in time, so

dL/dt = (0, 0, 0)

But we also found

τ(t) = (0, 0, 0)

Therefore,

τ = dL/dt

So the relation is verified for uniform circular motion.

---

## 9. Physical interpretation

Angular momentum measures the rotational motion of the particle about the origin.

In uniform circular motion:

- the radius is constant
- the speed is constant
- the angular momentum magnitude is constant
- the angular momentum direction is fixed

Because the centripetal force is directed exactly toward the center, it has no lever arm about the origin in the tangential sense, so it produces no torque about the origin.

That is why the angular momentum stays constant.

---

## Final Answers

### Velocity

v(t) = (-Rω sin(ωt), Rω cos(ωt), 0)

### Angular momentum

L(t) = m r(t) × v(t) = (0, 0, mR^2ω)

### Magnitude

|L| = mR^2ω

This is constant.

### Direction

L is perpendicular to the xy-plane and points in the positive z-direction for counterclockwise motion.

### Centripetal force

F(t) = -mω^2 r(t)

### Torque

τ(t) = r(t) × F(t) = 0

### Verification

dL/dt = 0 = τ

So the relation

τ = dL/dt

is satisfied.

---

## Short geometric summary

- r lies in the xy-plane
- v is tangent to the circle in the xy-plane
- r × v is perpendicular to both r and v
- therefore L is along the z-axis
- its magnitude is mR^2ω
