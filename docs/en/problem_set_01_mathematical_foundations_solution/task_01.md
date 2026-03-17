# Problem 1 – Vectors and Linear Transformations

## Given

\[
\vec a = (2, -1, 3), \quad \vec b = (1, 4, -2)
\]

\[
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
\]

---

# 1. Lengths of the vectors

## Length of \(\vec a\)

\[
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2}
= \sqrt{4 + 1 + 9}
= \sqrt{14}
\]

## Length of \(\vec b\)

\[
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2}
= \sqrt{1 + 16 + 4}
= \sqrt{21}
\]

---

# 2. Normalized vector

\[
\hat a = \frac{\vec a}{|\vec a|}
= \frac{(2, -1, 3)}{\sqrt{14}}
= \left(\frac{2}{\sqrt{14}}, \frac{-1}{\sqrt{14}}, \frac{3}{\sqrt{14}}\right)
\]

---

# 3. Dot product and angle

## Dot product

\[
\vec a \cdot \vec b = (2)(1) + (-1)(4) + (3)(-2)
= 2 - 4 - 6
= -8
\]

## Angle between vectors

\[
\cos \theta = \frac{\vec a \cdot \vec b}{|\vec a||\vec b|}
= \frac{-8}{\sqrt{14}\sqrt{21}}
= \frac{-8}{\sqrt{294}}
\]

\[
\theta = \cos^{-1}\left(\frac{-8}{\sqrt{294}}\right)
\approx 117.9^\circ
\]

---

# 4. Cross product and area

## Cross product

\[
\vec a \times \vec b =
\begin{vmatrix}
\mathbf i & \mathbf j & \mathbf k \\
2 & -1 & 3 \\
1 & 4 & -2
\end{vmatrix}
\]

\[
= \mathbf i((-1)(-2) - 3 \cdot 4)
- \mathbf j(2(-2) - 3 \cdot 1)
+ \mathbf k(2 \cdot 4 - (-1) \cdot 1)
\]

\[
= \mathbf i(2 - 12)
- \mathbf j(-4 - 3)
+ \mathbf k(8 + 1)
\]

\[
= (-10, 7, 9)
\]

## Area of parallelogram

\[
|\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2}
= \sqrt{100 + 49 + 81}
= \sqrt{230}
\approx 15.17
\]

---

# 5. Matrix multiplication \(A\vec a\)

\[
A \vec a =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
-1 \\
3
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2 \cdot 2 + 1 \cdot (-1) + 0 \cdot 3 \\
0 \cdot 2 + 1 \cdot (-1) + (-1) \cdot 3 \\
1 \cdot 2 + 0 \cdot (-1) + 1 \cdot 3
\end{pmatrix}
=
\begin{pmatrix}
3 \\
-4 \\
5
\end{pmatrix}
\]

---

# 6. Determinant of \(A\)

\[
\det A =
2
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
- 1
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
+ 0
\]

\[
= 2(1 \cdot 1 - (-1) \cdot 0)
- (0 \cdot 1 - (-1) \cdot 1)
\]

\[
= 2(1) - (1)
= 1
\]

---

# 7. Orientation

Since

\[
\det A = 1 > 0
\]

the transformation **preserves orientation**.

---

# Final Results

- \(|\vec a| = \sqrt{14}\), \(|\vec b| = \sqrt{21}\)
- \(\hat a = \left(\frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}}\right)\)
- \(\vec a \cdot \vec b = -8\)
- \(\theta \approx 117.9^\circ\)
- \(\vec a \times \vec b = (-10, 7, 9)\)
- Area \(= \sqrt{230}\)
- \(A\vec a = (3, -4, 5)\)
- \(\det A = 1\)
- Orientation is preserved
