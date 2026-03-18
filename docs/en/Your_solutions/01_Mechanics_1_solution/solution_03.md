# Path Intersection — Theory + Solution

---

# Useful Definitions and Formulas

### 1. Parametric Motion

The position of a moving object in the plane is given by:

$$
\vec{r}(t)=(x(t),y(t))
$$

Two objects **collide** if their positions are equal at the same time:

$$
A(t)=B(t)
$$

---

### 2. Condition for Intersection

We must solve the system:

$$
x_A(t)=x_B(t)
$$

$$
y_A(t)=y_B(t)
$$

If a **single value of $t$ satisfies both equations**, the objects collide.

---

### 3. Distance Between Two Points

If no collision occurs, the distance between them is:

$$
d(t)=\sqrt{(x_A-x_B)^2+(y_A-y_B)^2}
$$

To minimize distance, minimize:

$$
d^2(t)=(x_A-x_B)^2+(y_A-y_B)^2
$$

---

### 4. Optimization

Find minimum distance by:

$$
\frac{d}{dt}d^2(t)=0
$$

---

# Step-by-Step Solution

Given:

$$
A(t)=(2+t,\ 8-3t)
$$

$$
B(t)=(2t-1,\ 2t+2)
$$

---

# Step 1. Check for Collision

Set coordinates equal.

### X-coordinate:

$$
2+t=2t-1
$$

Solve:

$$
2+t=2t-1
$$

$$
2+1=2t-t
$$

$$
3=t
$$

---

### Y-coordinate:

$$
8-3t=2t+2
$$

Substitute $t=3$:

$$
8-3\cdot3=2\cdot3+2
$$

$$
8-9=6+2
$$

$$
-1\neq8
$$

---

### Conclusion

The same $t$ does **not** satisfy both equations.

$$
\text{No collision occurs}
$$

---

# Step 2. Distance Between Alice and Bob

Compute differences:

$$
x_A-x_B=(2+t)-(2t-1)=2+t-2t+1=3-t
$$

$$
y_A-y_B=(8-3t)-(2t+2)=8-3t-2t-2=6-5t
$$

---

### Distance squared:

$$
d^2(t)=(3-t)^2+(6-5t)^2
$$

Expand:

$$
(3-t)^2=9-6t+t^2
$$

$$
(6-5t)^2=36-60t+25t^2
$$

---

### Combine:

$$
d^2(t)=9-6t+t^2+36-60t+25t^2
$$

$$
d^2(t)=45-66t+26t^2
$$

---

# Step 3. Minimize Distance

Differentiate:

$$
\frac{d}{dt}d^2(t)=52t-66
$$

Set equal to zero:

$$
52t-66=0
$$

$$
t=\frac{66}{52}=\frac{33}{26}
$$

---

# Step 4. Minimum Distance

Substitute into $d^2(t)$:

$$
d^2=\left(3-\frac{33}{26}\right)^2+\left(6-5\cdot\frac{33}{26}\right)^2
$$

Simplify:

$$
3=\frac{78}{26}
$$

$$
3-\frac{33}{26}=\frac{45}{26}
$$

---

Second term:

$$
6=\frac{156}{26}
$$

$$
6-\frac{165}{26}=\frac{-9}{26}
$$

---

Thus:

$$
d^2=\left(\frac{45}{26}\right)^2+\left(\frac{-9}{26}\right)^2
$$

$$
d^2=\frac{2025}{676}+\frac{81}{676}
$$

$$
d^2=\frac{2106}{676}
$$

---

### Distance:

$$
d=\sqrt{\frac{2106}{676}}=\frac{\sqrt{2106}}{26}
$$

Approximation:

$$
d\approx1.77
$$

---

# Final Answers

### Collision:
$$
\text{No collision}
$$

---

### Time of closest approach:
$$
t=\frac{33}{26}\approx1.27
$$

---

### Minimum distance:
$$
d=\frac{\sqrt{2106}}{26}\approx1.77
$$

---

# Comments

- The paths intersect geometrically, but **not at the same time**, so no collision.
- Minimizing $d^2(t)$ avoids dealing with square roots.
- This is a standard quadratic minimization problem.