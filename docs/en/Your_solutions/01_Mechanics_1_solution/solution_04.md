# Vector Calculus — Detailed Theory + Solution

---

# Useful Definitions and Concepts

### 1. What is a Vector?

A **vector** is a quantity that has:
- magnitude (length)
- direction

In 2D space, a vector is written as:

$$
\vec{r}=x\hat{i}+y\hat{j}
$$

where:
- $\hat{i}$ — unit vector along x-axis
- $\hat{j}$ — unit vector along y-axis

---

### 2. Position Vector

The position of a particle is:

$$
\vec{r}(t)=x(t)\hat{i}+y(t)\hat{j}
$$

It tells us **where the object is at time $t$**.

---

### 3. Velocity Vector

Velocity describes how position changes:

$$
\vec{v}(t)=\frac{d\vec{r}(t)}{dt}
$$

This means:
- direction of motion
- speed of change

---

### 4. Acceleration Vector

Acceleration describes how velocity changes:

$$
\vec{a}(t)=\frac{d\vec{v}(t)}{dt}
$$

---

### 5. Power Rule

$$
\frac{d}{dt}t^n=nt^{n-1}
$$

---

# Visual Representation (Concept)

- $\vec{r}(t)$ → arrow from origin to point  
- $\vec{v}(t)$ → tangent to trajectory  
- $\vec{a}(t)$ → shows how motion changes  

---


::contentReference[oaicite:0]{index=0}


---

# Step-by-Step Solution

Given:

$$
\vec{r}(t)=(3t^2)\hat{i}+(5t-8t^2)\hat{j}
$$

---

# Step 1. Identify Components

$$
x(t)=3t^2
$$

$$
y(t)=5t-8t^2
$$

---

# Step 2. Find Velocity Vector

Differentiate each component.

### X-component:

$$
\frac{dx}{dt}=6t
$$

---

### Y-component:

$$
\frac{dy}{dt}=5-16t
$$

---

### Velocity:

$$
\vec{v}(t)=6t\hat{i}+(5-16t)\hat{j}
$$

---

# Step 3. Find Acceleration Vector

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

### Acceleration:

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

# Comments and Physical Meaning

- Velocity changes with time → motion is **non-uniform**
- Acceleration is constant → motion has **uniform acceleration**
- The object follows a **curved path (parabola)**

---

# Intuition

- $\vec{r}(t)$ → where the object is  
- $\vec{v}(t)$ → where it is going  
- $\vec{a}(t)$ → how its motion is changing  