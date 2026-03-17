# Problem 1 – Vectors and Linear Transformations

## Given

**Vectors:**

- a = (2, -1, 3)  
- b = (1, 4, -2)

**Matrix:**

A = | 2 1 0 |
| 0 1 -1 |
| 1 0 1 |


---

## 1. Lengths of the vectors

### Length of a

|a| = √(2² + (-1)² + 3²)  
|a| = √(4 + 1 + 9)  
|a| = √14  

### Length of b

|b| = √(1² + 4² + (-2)²)  
|b| = √(1 + 16 + 4)  
|b| = √21  

---

## 2. Normalized vector

â = a / |a|  

â = (2, -1, 3) / √14  

â = (2/√14, -1/√14, 3/√14)

---

## 3. Dot product and angle

### Dot product

a · b = (2)(1) + (-1)(4) + (3)(-2)  
a · b = 2 - 4 - 6  
a · b = -8  

### Angle between vectors

cos(θ) = (a · b) / (|a||b|)  

cos(θ) = -8 / (√14 · √21)  
cos(θ) = -8 / √294  

θ = arccos(-8 / √294) ≈ 117.9°

---

## 4. Cross product and area

### Cross product

| i j k |
| 2 -1 3 |
| 1 4 -2 |


a × b =  

= i((-1)(-2) - 3·4)  
- j(2(-2) - 3·1)  
+ k(2·4 - (-1)·1)

= i(2 - 12) - j(-4 - 3) + k(8 + 1)  

= (-10, 7, 9)

### Area of parallelogram

|a × b| = √((-10)² + 7² + 9²)  
|a × b| = √(100 + 49 + 81)  
|a × b| = √230 ≈ 15.17  

---

## 5. Matrix multiplication A · a

A = | 2 1 0 |
| 0 1 -1 |
| 1 0 1 |

a = | 2 |
| -1 |
| 3 |


A · a =  

= (2·2 + 1·(-1) + 0·3,  
   0·2 + 1·(-1) + (-1)·3,  
   1·2 + 0·(-1) + 1·3)

= (3, -4, 5)

---

## 6. Determinant of A

det(A) =  

= 2 * | 1  -1 |  
      | 0   1 |

- 1 * | 0  -1 |  
      | 1   1 |

+ 0  

= 2(1·1 - (-1)·0) - (0·1 - (-1)·1)  

= 2(1) - (1)  

= 1  

---

## 7. Orientation

Since det(A) = 1 > 0  

The transformation **preserves orientation**

---

## Final Results

- |a| = √14  
- |b| = √21  
- â = (2/√14, -1/√14, 3/√14)  
- a · b = -8  
- θ ≈ 117.9°  
- a × b = (-10, 7, 9)  
- Area = √230 ≈ 15.17  
- A · a = (3, -4, 5)  
- det(A) = 1  
- Orientation preserved
