# Elimination of Time and Acceleration — Theory + Solution

---

# Useful Definitions and Formulas

### 1. Parametric Equations

A curve can be described as:

$$
x=x(t),\quad y=y(t)
$$

To eliminate $t$, express $t$ from one equation and substitute into the other.

---

### 2. Velocity Vector

$$
\vec{v}(t)=\frac{d\vec{r}(t)}{dt}
$$

$$
\vec{v}(t)=\frac{dx}{dt}\hat{i}+\frac{dy}{dt}\hat{j}
$$

---

### 3. Speed (Magnitude of Velocity)

$$
|\vec{v}(t)|=\sqrt{\left(\frac{dx}{dt}\right)^2+\left(\frac{dy}{dt}\right)^2}
$$

---

### 4. Acceleration Vector

$$
\vec{a}(t)=\frac{d^2\vec{r}(t)}{dt^2}
$$

---

### 5. Magnitude of Acceleration

$$
|\vec{a}(t)|=\sqrt{a_x^2+a_y^2}
$$

---

# Step-by-Step Solution

Given:

$$
x(t)=2t^2,\quad y(t)=3t^3
$$

---

# 1. Eliminate the Parameter $t$

From $x(t)$:

$$
x=2t^2
$$

$$
t^2=\frac{x}{2}
$$

$$
t=\sqrt{\frac{x}{2}}
$$

---

Substitute into $y(t)$:

$$
y=3t^3=3t\cdot t^2
$$

$$
y=3\cdot\sqrt{\frac{x}{2}}\cdot\frac{x}{2}
$$

---

Simplify:

$$
y=\frac{3x}{2}\sqrt{\frac{x}{2}}
$$

---

# Trajectory Equation

$$
y=\frac{3x}{2}\sqrt{\frac{x}{2}}
$$

---

# 2. Interpretation of the Trajectory

- This is a **nonlinear curve**
- It behaves like $y\sim x^{3/2}$
- The motion is not symmetric (unlike a parabola)

---

# 3. Velocity Vector

Differentiate components:

### X-component:

$$
\frac{dx}{dt}=4t
$$

---

### Y-component:

$$
\frac{dy}{dt}=9t^2
$$

---

### Velocity:

$$
\vec{v}(t)=4t\hat{i}+9t^2\hat{j}
$$

---

# 4. Speed

$$
|\vec{v}(t)|=\sqrt{(4t)^2+(9t^2)^2}
$$

$$
|\vec{v}(t)|=\sqrt{16t^2+81t^4}
$$

Factor:

$$
|\vec{v}(t)|=\sqrt{t^2(16+81t^2)}
$$

$$
|\vec{v}(t)|=|t|\sqrt{16+81t^2}
$$

---

# 5. Acceleration Vector

Differentiate velocity:

### X-component:

$$
\frac{d}{dt}(4t)=4
$$

---

### Y-component:

$$
\frac{d}{dt}(9t^2)=18t
$$

---

### Acceleration:

$$
\vec{a}(t)=4\hat{i}+18t\hat{j}
$$

---

# 6. Magnitude of Acceleration

$$
|\vec{a}(t)|=\sqrt{4^2+(18t)^2}
$$

$$
|\vec{a}(t)|=\sqrt{16+324t^2}
$$

---

# 7. Is Acceleration Constant?

- X-component is constant: $4$
- Y-component depends on time: $18t$

---

### Conclusion:

$$
\vec{a}(t)\ \text{is NOT constant}
$$

---

# Final Answers

### Trajectory:

$$
y=\frac{3x}{2}\sqrt{\frac{x}{2}}
$$

---

### Velocity:

$$
\vec{v}(t)=4t\hat{i}+9t^2\hat{j}
$$

---

### Speed:

$$
|\vec{v}(t)|=|t|\sqrt{16+81t^2}
$$

---

### Acceleration:

$$
\vec{a}(t)=4\hat{i}+18t\hat{j}
$$

---

### Magnitude of acceleration:

$$
|\vec{a}(t)|=\sqrt{16+324t^2}
$$

---

### Acceleration nature:

$$
\text{Non-constant acceleration}
$$

---

# Comments

- Motion becomes faster as $t$ increases due to growing velocity components.
- Acceleration increases in the $y$-direction → trajectory curves more sharply over time.
- This is a classic example of **non-uniform accelerated motion**.