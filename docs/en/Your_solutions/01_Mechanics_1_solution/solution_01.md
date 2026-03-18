# Solutions goes here

...# Projectile Motion — Theory + Solution

---

# Useful Definitions and Formulas

### 1. Decomposition of Initial Velocity

The initial velocity $v_0$ can be split into horizontal and vertical components:

$$
v_{0x}=v_0\cos\theta
$$

$$
v_{0y}=v_0\sin\theta
$$

---

### 2. Equations of Motion (Constant Acceleration)

From Newton’s Second Law:

$$
\frac{d^2x}{dt^2}=0
$$

$$
\frac{d^2y}{dt^2}=-g
$$

After integration:

$$
x(t)=v_{0x}t
$$

$$
y(t)=v_{0y}t-\frac{1}{2}gt^2
$$

---

### 3. Time of Flight

The projectile returns to the ground when $y=0$:

$$
T=\frac{2v_0\sin\theta}{g}
$$

---

### 4. Maximum Height

At the top point $v_y=0$:

$$
H=\frac{(v_0\sin\theta)^2}{2g}
$$

---

### 5. Range

Horizontal distance traveled:

$$
R=v_0\cos\theta \cdot T
$$

or:

$$
R=\frac{v_0^2\sin2\theta}{g}
$$

---

# Step-by-Step Solution

Given:

$$
v_0=100\ \text{m/s}
$$

$$
\theta=37^\circ
$$

$$
g=9.8\ \text{m/s}^2
$$

Use approximations:

$$
\sin37^\circ\approx0.6,\quad \cos37^\circ\approx0.8
$$

---

# 1. Differential Equations of Motion

### Horizontal direction:

$$
\frac{d^2x}{dt^2}=0
$$

Integrate:

$$
\frac{dx}{dt}=v_0\cos\theta=100\cdot0.8=80
$$

$$
x(t)=80t
$$

---

### Vertical direction:

$$
\frac{d^2y}{dt^2}=-g
$$

Integrate:

$$
\frac{dy}{dt}=v_0\sin\theta-gt=100\cdot0.6-9.8t=60-9.8t
$$

$$
y(t)=60t-4.9t^2
$$

---

# 2. Time of Flight

Use:

$$
T=\frac{2v_0\sin\theta}{g}
$$

Substitute:

$$
T=\frac{2\cdot100\cdot0.6}{9.8}
=\frac{120}{9.8}
\approx12.24\ \text{s}
$$

---

# 3. Maximum Height

Use:

$$
H=\frac{(v_0\sin\theta)^2}{2g}
$$

Substitute:

$$
H=\frac{(100\cdot0.6)^2}{2\cdot9.8}
=\frac{60^2}{19.6}
=\frac{3600}{19.6}
\approx183.67\ \text{m}
$$

---

# 4. Range

Use:

$$
R=v_0\cos\theta \cdot T
$$

Substitute:

$$
R=100\cdot0.8\cdot12.24
=80\cdot12.24
\approx979.2\ \text{m}
$$

---

# Final Answers

$$
T\approx12.24\ \text{s}
$$

$$
H\approx183.67\ \text{m}
$$

$$
R\approx979.2\ \text{m}
$$

---

# Comments

- Horizontal motion is uniform because no force acts along $x$.
- Vertical motion is uniformly accelerated due to gravity.
- The trajectory is a parabola.
- The motion is symmetric: time to rise = time to fall.