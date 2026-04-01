# 📘 Dynamics with Time-Dependent Force

---

## 🔑 Key Definitions and Formulas

### 📌 Newton’s Second Law

$$
\vec{F}=m\vec{a}
$$

So:

$$
\vec{a}=\frac{\vec{F}}{m}
$$

---

### 📌 Acceleration → Velocity

$$
\vec{v}(t)=\int \vec{a}(t)\,dt + \vec{C}
$$

---

### 📌 Velocity → Position

$$
\vec{r}(t)=\int \vec{v}(t)\,dt + \vec{C}
$$

---

## 🧩 Given:

- $m=3\ \text{kg}$

$$
\vec{F}(t)=(15t,\;3t-12,\;-6t^2)
$$

- Initial conditions:

$$
\vec{r}_0=(5,2,-3),\quad \vec{v}_0=(2,0,1)
$$

---

# 🔍 Step 1: Find Acceleration

$$
\vec{a}(t)=\frac{\vec{F}}{m}
$$

---

### 🔄 Compute components:

$$
a_x=\frac{15t}{3}=5t
$$

$$
a_y=\frac{3t-12}{3}=t-4
$$

$$
a_z=\frac{-6t^2}{3}=-2t^2
$$

---

### ✅ Acceleration:

$$
\vec{a}(t)=(5t,\;t-4,\;-2t^2)
$$

---

# 🔍 Step 2: Find Velocity

Integrate each component.

---

### 🔄 $v_x$:

$$
v_x=\int 5t\,dt=\frac{5}{2}t^2+C_1
$$

Apply $v_x(0)=2$:

$$
C_1=2
$$

$$
v_x=\frac{5}{2}t^2+2
$$

---

### 🔄 $v_y$:

$$
v_y=\int (t-4)\,dt=\frac{1}{2}t^2-4t+C_2
$$

Apply $v_y(0)=0$:

$$
C_2=0
$$

$$
v_y=\frac{1}{2}t^2-4t
$$

---

### 🔄 $v_z$:

$$
v_z=\int -2t^2\,dt=-\frac{2}{3}t^3+C_3
$$

Apply $v_z(0)=1$:

$$
C_3=1
$$

$$
v_z=-\frac{2}{3}t^3+1
$$

---

### ✅ Velocity:

$$
\vec{v}(t)=\left(\frac{5}{2}t^2+2,\;\frac{1}{2}t^2-4t,\;-\frac{2}{3}t^3+1\right)
$$

---

# 🔍 Step 3: Find Position

Integrate velocity.

---

### 🔄 $x(t)$:

$$
x=\int\left(\frac{5}{2}t^2+2\right)dt=\frac{5}{6}t^3+2t+C_4
$$

Apply $x(0)=5$:

$$
C_4=5
$$

$$
x=\frac{5}{6}t^3+2t+5
$$

---

### 🔄 $y(t)$:

$$
y=\int\left(\frac{1}{2}t^2-4t\right)dt=\frac{1}{6}t^3-2t^2+C_5
$$

Apply $y(0)=2$:

$$
C_5=2
$$

$$
y=\frac{1}{6}t^3-2t^2+2
$$

---

### 🔄 $z(t)$:

$$
z=\int\left(-\frac{2}{3}t^3+1\right)dt=-\frac{1}{6}t^4+t+C_6
$$

Apply $z(0)=-3$:

$$
C_6=-3
$$

$$
z=-\frac{1}{6}t^4+t-3
$$

---

### ✅ Position:

$$
\vec{r}(t)=\left(\frac{5}{6}t^3+2t+5,\;\frac{1}{6}t^3-2t^2+2,\;-\frac{1}{6}t^4+t-3\right)
$$

---

# 🎯 Final Results

- Velocity:

$$
\vec{v}(t)=\left(\frac{5}{2}t^2+2,\;\frac{1}{2}t^2-4t,\;-\frac{2}{3}t^3+1\right)
$$

- Position:

$$
\vec{r}(t)=\left(\frac{5}{6}t^3+2t+5,\;\frac{1}{6}t^3-2t^2+2,\;-\frac{1}{6}t^4+t-3\right)
$$

---