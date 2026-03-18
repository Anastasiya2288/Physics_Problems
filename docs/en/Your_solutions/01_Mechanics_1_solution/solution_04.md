# Vector Calculus — Theory + Solution

---

# Useful Definitions and Formulas

### 1. Position Vector

The position of a particle in 2D is:

$$
\vec{r}(t)=x(t)\hat{i}+y(t)\hat{j}
$$

---

### 2. Velocity Vector

Velocity is the **first derivative** of position:

$$
\vec{v}(t)=\frac{d\vec{r}(t)}{dt}
$$

This means we differentiate each component:

$$
\vec{v}(t)=\frac{dx}{dt}\hat{i}+\frac{dy}{dt}\hat{j}
$$

---

### 3. Acceleration Vector

Acceleration is the **second derivative** of position (or derivative of velocity):

$$
\vec{a}(t)=\frac{d\vec{v}(t)}{dt}=\frac{d^2\vec{r}(t)}{dt^2}
$$

---

### 4. Power Rule for Differentiation

$$
\frac{d}{dt}t^n=nt^{n-1}
$$

---

# Step-by-Step Solution

Given:

$$
\vec{r}(t)=(3t^2)\hat{i}+(5t-8t^2)\hat{j}
$$

---

# Step 1. Find Velocity Vector

Differentiate each component.

### X-component:

$$
\frac{d}{dt}(3t^2)=6t
$$

---

### Y-component:

$$
\frac{d}{dt}(5t-8t^2)=5-16t
$$

---

### Velocity vector:

$$
\vec{v}(t)=6t\hat{i}+(5-16t)\hat{j}
$$

---

# Step 2. Find Acceleration Vector

Differentiate velocity.

### X-component:

$$
\frac{d}{dt}(6t)=6
$$

---

### Y-component:

$$
\frac{d}{dt}(5-16t)=-16
$$

---

### Acceleration vector:

$$
\vec{a}(t)=6\hat{i}-16\hat{j}
$$

---

# Final Answers

### Velocity:

$$
\vec{v}(t)=6t\hat{i}+(5-16t)\hat{j}
$$

---

### Acceleration:

$$
\vec{a}(t)=6\hat{i}-16\hat{j}
$$

---

# Comments

- Velocity depends on time → motion is **non-uniform**.
- Acceleration is constant → motion has **constant acceleration**.
- The trajectory is a **parabolic curve** in the plane.