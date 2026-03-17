Problem 1 – Vectors and Linear Transformations

We are given

𝑎
⃗
=
(
2
,
−
1
,
3
)
,
𝑏
⃗
=
(
1
,
4
,
−
2
)
a
=(2,−1,3),
b
=(1,4,−2)

and the matrix

𝐴
=
(
2
	
1
	
0


0
	
1
	
−
1


1
	
0
	
1
)
A=
	​

2
0
1
	​

1
1
0
	​

0
−1
1
	​

	​


We will solve each part carefully.

1) Lengths of the vectors 
∣
𝑎
⃗
∣
∣
a
∣ and 
∣
𝑏
⃗
∣
∣
b
∣
Length of 
𝑎
⃗
a

For a vector 
(
𝑥
,
𝑦
,
𝑧
)
(x,y,z), the length is

∣
𝑣
⃗
∣
=
𝑥
2
+
𝑦
2
+
𝑧
2
∣
v
∣=
x
2
+y
2
+z
2
	​


So for 
𝑎
⃗
=
(
2
,
−
1
,
3
)
a
=(2,−1,3),

∣
𝑎
⃗
∣
=
2
2
+
(
−
1
)
2
+
3
2
∣
a
∣=
2
2
+(−1)
2
+3
2
	​


Now calculate each square:

2
2
=
4
,
(
−
1
)
2
=
1
,
3
2
=
9
2
2
=4,(−1)
2
=1,3
2
=9

Add them:

4
+
1
+
9
=
14
4+1+9=14

So

∣
𝑎
⃗
∣
=
14
∣
a
∣=
14
	​

Length of 
𝑏
⃗
b

For 
𝑏
⃗
=
(
1
,
4
,
−
2
)
b
=(1,4,−2),

∣
𝑏
⃗
∣
=
1
2
+
4
2
+
(
−
2
)
2
∣
b
∣=
1
2
+4
2
+(−2)
2
	​


Calculate each square:

1
2
=
1
,
4
2
=
16
,
(
−
2
)
2
=
4
1
2
=1,4
2
=16,(−2)
2
=4

Add them:

1
+
16
+
4
=
21
1+16+4=21

So

∣
𝑏
⃗
∣
=
21
∣
b
∣=
21
	​

Final answers for lengths
∣
𝑎
⃗
∣
=
14
,
∣
𝑏
⃗
∣
=
21
∣
a
∣=
14
	​

	​

,
∣
b
∣=
21
	​

	​

2) Normalized vector 
𝑎
^
=
𝑎
⃗
∣
𝑎
⃗
∣
a
^
=
∣
a
∣
a
	​


A normalized vector has length 1 and is found by dividing the vector by its magnitude.

We already found

∣
𝑎
⃗
∣
=
14
∣
a
∣=
14
	​


So

𝑎
^
=
𝑎
⃗
∣
𝑎
⃗
∣
=
(
2
,
−
1
,
3
)
14
a
^
=
∣
a
∣
a
	​

=
14
	​

(2,−1,3)
	​


Divide each component by 
14
14
	​

:

𝑎
^
=
(
2
14
,
−
1
14
,
3
14
)
a
^
=(
14
	​

2
	​

,
14
	​

−1
	​

,
14
	​

3
	​

)

So

𝑎
^
=
(
2
14
,
−
1
14
,
3
14
)
a
^
=(
14
	​

2
	​

,−
14
	​

1
	​

,
14
	​

3
	​

)
	​

3) Dot product 
𝑎
⃗
⋅
𝑏
⃗
a
⋅
b
 and the angle between the vectors
Step 1: Compute the dot product

The dot product formula is

𝑎
⃗
⋅
𝑏
⃗
=
𝑎
1
𝑏
1
+
𝑎
2
𝑏
2
+
𝑎
3
𝑏
3
a
⋅
b
=a
1
	​

b
1
	​

+a
2
	​

b
2
	​

+a
3
	​

b
3
	​


Substitute the coordinates:

𝑎
⃗
⋅
𝑏
⃗
=
(
2
)
(
1
)
+
(
−
1
)
(
4
)
+
(
3
)
(
−
2
)
a
⋅
b
=(2)(1)+(−1)(4)+(3)(−2)

Now calculate each term:

(
2
)
(
1
)
=
2
,
(
−
1
)
(
4
)
=
−
4
,
(
3
)
(
−
2
)
=
−
6
(2)(1)=2,(−1)(4)=−4,(3)(−2)=−6

Add them:

2
+
(
−
4
)
+
(
−
6
)
=
2
−
4
−
6
=
−
8
2+(−4)+(−6)=2−4−6=−8

So

𝑎
⃗
⋅
𝑏
⃗
=
−
8
a
⋅
b
=−8
	​

Step 2: Use the dot product formula for the angle

The angle 
𝜃
θ between two vectors satisfies

𝑎
⃗
⋅
𝑏
⃗
=
∣
𝑎
⃗
∣
∣
𝑏
⃗
∣
cos
⁡
𝜃
a
⋅
b
=∣
a
∣∣
b
∣cosθ

So

cos
⁡
𝜃
=
𝑎
⃗
⋅
𝑏
⃗
∣
𝑎
⃗
∣
∣
𝑏
⃗
∣
cosθ=
∣
a
∣∣
b
∣
a
⋅
b
	​


Substitute the values:

cos
⁡
𝜃
=
−
8
14
21
cosθ=
14
	​

21
	​

−8
	​


Combine the square roots:

14
21
=
294
14
	​

21
	​

=
294
	​


So

cos
⁡
𝜃
=
−
8
294
cosθ=
294
	​

−8
	​


Thus

𝜃
=
cos
⁡
−
1
(
−
8
294
)
θ=cos
−1
(
294
	​

−8
	​

)

This is the exact answer.

Step 3: Approximate the angle
294
≈
17.146
294
	​

≈17.146

So

cos
⁡
𝜃
≈
−
8
17.146
≈
−
0.467
cosθ≈
17.146
−8
	​

≈−0.467

Then

𝜃
≈
cos
⁡
−
1
(
−
0.467
)
≈
117.9
∘
θ≈cos
−1
(−0.467)≈117.9
∘

So the angle is approximately

𝜃
≈
117.9
∘
θ≈117.9
∘
	​

Final answers for dot product and angle
𝑎
⃗
⋅
𝑏
⃗
=
−
8
a
⋅
b
=−8
	​

𝜃
=
cos
⁡
−
1
(
−
8
294
)
≈
117.9
∘
θ=cos
−1
(
294
	​

−8
	​

)≈117.9
∘
	​

4) Cross product 
𝑎
⃗
×
𝑏
⃗
a
×
b
 and area of the parallelogram
Step 1: Write the determinant form

The cross product is

𝑎
⃗
×
𝑏
⃗
=
∣
𝑖
	
𝑗
	
𝑘


2
	
−
1
	
3


1
	
4
	
−
2
∣
a
×
b
=
	​

i
2
1
	​

j
−1
4
	​

k
3
−2
	​

	​


Expand along the first row:

𝑎
⃗
×
𝑏
⃗
=
𝑖
∣
−
1
	
3


4
	
−
2
∣
−
𝑗
∣
2
	
3


1
	
−
2
∣
+
𝑘
∣
2
	
−
1


1
	
4
∣
a
×
b
=i
	​

−1
4
	​

3
−2
	​

	​

−j
	​

2
1
	​

3
−2
	​

	​

+k
	​

2
1
	​

−1
4
	​

	​

Step 2: Compute each 
2
×
2
2×2 determinant
𝑖
i-component
∣
−
1
	
3


4
	
−
2
∣
=
(
−
1
)
(
−
2
)
−
(
3
)
(
4
)
=
2
−
12
=
−
10
	​

−1
4
	​

3
−2
	​

	​

=(−1)(−2)−(3)(4)=2−12=−10
𝑗
j-component
∣
2
	
3


1
	
−
2
∣
=
(
2
)
(
−
2
)
−
(
3
)
(
1
)
=
−
4
−
3
=
−
7
	​

2
1
	​

3
−2
	​

	​

=(2)(−2)−(3)(1)=−4−3=−7

Because of the minus sign in front of 
𝑗
j,

−
𝑗
(
−
7
)
=
+
7
𝑗
−j(−7)=+7j
𝑘
k-component
∣
2
	
−
1


1
	
4
∣
=
(
2
)
(
4
)
−
(
−
1
)
(
1
)
=
8
−
(
−
1
)
=
9
	​

2
1
	​

−1
4
	​

	​

=(2)(4)−(−1)(1)=8−(−1)=9
Step 3: Write the cross product
𝑎
⃗
×
𝑏
⃗
=
−
10
𝑖
+
7
𝑗
+
9
𝑘
a
×
b
=−10i+7j+9k

So in vector form,

𝑎
⃗
×
𝑏
⃗
=
(
−
10
,
7
,
9
)
a
×
b
=(−10,7,9)
	​

Step 4: Area of the parallelogram

The area of the parallelogram spanned by 
𝑎
⃗
a
 and 
𝑏
⃗
b
 is the magnitude of the cross product:

Area
=
∣
𝑎
⃗
×
𝑏
⃗
∣
Area=∣
a
×
b
∣

So

∣
𝑎
⃗
×
𝑏
⃗
∣
=
(
−
10
)
2
+
7
2
+
9
2
∣
a
×
b
∣=
(−10)
2
+7
2
+9
2
	​


Compute the squares:

(
−
10
)
2
=
100
,
7
2
=
49
,
9
2
=
81
(−10)
2
=100,7
2
=49,9
2
=81

Add them:

100
+
49
+
81
=
230
100+49+81=230

Thus

∣
𝑎
⃗
×
𝑏
⃗
∣
=
230
∣
a
×
b
∣=
230
	​


So the area is

230
230
	​

	​


Approximate value:

230
≈
15.17
230
	​

≈15.17
Final answers for cross product and area
𝑎
⃗
×
𝑏
⃗
=
(
−
10
,
7
,
9
)
a
×
b
=(−10,7,9)
	​

Area of parallelogram
=
230
≈
15.17
Area of parallelogram=
230
	​

≈15.17
	​

5) Calculate 
𝐴
𝑎
⃗
A
a

We have

𝐴
=
(
2
	
1
	
0


0
	
1
	
−
1


1
	
0
	
1
)
,
𝑎
⃗
=
(
2


−
1


3
)
A=
	​

2
0
1
	​

1
1
0
	​

0
−1
1
	​

	​

,
a
=
	​

2
−1
3
	​

	​


We multiply row by column.

First component
(
2
)
(
2
)
+
(
1
)
(
−
1
)
+
(
0
)
(
3
)
(2)(2)+(1)(−1)+(0)(3)
=
4
−
1
+
0
=
3
=4−1+0=3
Second component
(
0
)
(
2
)
+
(
1
)
(
−
1
)
+
(
−
1
)
(
3
)
(0)(2)+(1)(−1)+(−1)(3)
=
0
−
1
−
3
=
−
4
=0−1−3=−4
Third component
(
1
)
(
2
)
+
(
0
)
(
−
1
)
+
(
1
)
(
3
)
(1)(2)+(0)(−1)+(1)(3)
=
2
+
0
+
3
=
5
=2+0+3=5
Result
𝐴
𝑎
⃗
=
(
3


−
4


5
)
A
a
=
	​

3
−4
5
	​

	​


So

𝐴
𝑎
⃗
=
(
3
,
−
4
,
5
)
A
a
=(3,−4,5)
	​

6) Calculate 
det
⁡
𝐴
detA

We compute the determinant of

𝐴
=
(
2
	
1
	
0


0
	
1
	
−
1


1
	
0
	
1
)
A=
	​

2
0
1
	​

1
1
0
	​

0
−1
1
	​

	​


Expand along the first row:

det
⁡
𝐴
=
2
∣
1
	
−
1


0
	
1
∣
−
1
∣
0
	
−
1


1
	
1
∣
+
0
∣
0
	
1


1
	
0
∣
detA=2
	​

1
0
	​

−1
1
	​

	​

−1
	​

0
1
	​

−1
1
	​

	​

+0
	​

0
1
	​

1
0
	​

	​


Now compute each determinant.

First minor
∣
1
	
−
1


0
	
1
∣
=
(
1
)
(
1
)
−
(
−
1
)
(
0
)
=
1
−
0
=
1
	​

1
0
	​

−1
1
	​

	​

=(1)(1)−(−1)(0)=1−0=1

So the first term is

2
(
1
)
=
2
2(1)=2
Second minor
∣
0
	
−
1


1
	
1
∣
=
(
0
)
(
1
)
−
(
−
1
)
(
1
)
=
0
−
(
−
1
)
=
1
	​

0
1
	​

−1
1
	​

	​

=(0)(1)−(−1)(1)=0−(−1)=1

Because of the minus sign in expansion:

−
1
(
1
)
=
−
1
−1(1)=−1
Third term
0
⋅
(
anything
)
=
0
0⋅(anything)=0
Add all terms
det
⁡
𝐴
=
2
−
1
+
0
=
1
detA=2−1+0=1

So

det
⁡
𝐴
=
1
detA=1
	​

7) Does the transformation preserve orientation?

A linear transformation preserves orientation if its determinant is positive.

If 
det
⁡
𝐴
>
0
detA>0, orientation is preserved.

If 
det
⁡
𝐴
<
0
detA<0, orientation is reversed.

We found

det
⁡
𝐴
=
1
>
0
detA=1>0

Therefore, the transformation preserves orientation.

Yes, the transformation preserves orientation.
Yes, the transformation preserves orientation.
	​

Final summary
Vector lengths
∣
𝑎
⃗
∣
=
14
,
∣
𝑏
⃗
∣
=
21
∣
a
∣=
14
	​

	​

,
∣
b
∣=
21
	​

	​

Normalized vector
𝑎
^
=
(
2
14
,
−
1
14
,
3
14
)
a
^
=(
14
	​

2
	​

,−
14
	​

1
	​

,
14
	​

3
	​

)
	​

Dot product and angle
𝑎
⃗
⋅
𝑏
⃗
=
−
8
a
⋅
b
=−8
	​

𝜃
=
cos
⁡
−
1
(
−
8
294
)
≈
117.9
∘
θ=cos
−1
(
294
	​

−8
	​

)≈117.9
∘
	​

Cross product and parallelogram area
𝑎
⃗
×
𝑏
⃗
=
(
−
10
,
7
,
9
)
a
×
b
=(−10,7,9)
	​

Area
=
230
≈
15.17
Area=
230
	​

≈15.17
	​

Matrix action
𝐴
𝑎
⃗
=
(
3
,
−
4
,
5
)
A
a
=(3,−4,5)
	​

Determinant
det
⁡
𝐴
=
1
detA=1
	​

Orientation
Orientation is preserved
Orientation is preserved
	​
