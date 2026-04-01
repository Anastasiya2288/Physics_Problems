# 📘 Work and Energy with a Constant Force (2D Motion)

---

## 🔑 Key Definitions and Formulas

### 📌 Newton’s Second Law

$$
\vec{F}=m\vec{a}\quad\Rightarrow\quad \vec{a}=\frac{\vec{F}}{m}
$$

---

### 📌 Velocity from Acceleration

$$
\vec{v}(t)=\vec{v}_0+\vec{a}t
$$

---

### 📌 Position from Velocity

$$
\vec{r}(t)=\vec{r}_0+\vec{v}_0 t+\frac{1}{2}\vec{a}t^2
$$

---

### 📌 Work by a Constant Force

$$
W=\vec{F}\cdot\Delta\vec{r}
$$

---

### 📌 Work–Energy Theorem

$$
W=\Delta K=\frac{1}{2}m v^2-\frac{1}{2}m v_0^2
$$

---

## 🧩 Given:

- $m=2\ \text{kg}$
- $\vec{F}=(6,2)\ \text{N}$
- $\vec{v}_0=(1,-1)\ \text{m/s}$
- $\vec{r}_0=(0,0)$

---

# 🔍 Step 1: Acceleration

$$
\vec{a}=\frac{\vec{F}}{m}=\left(\frac{6}{2},\frac{2}{2}\right)=(3,1)
$$

---

### ✅ Answer:

$$
\vec{a}(t)=(3,1)
$$

---

# 🔍 Step 2: Velocity

$$
\vec{v}(t)=\vec{v}_0+\vec{a}t
$$

---

### 🔄 Substitute:

$$
\vec{v}(t)=(1,-1)+(3t,t)
$$

---

### ✅ Result:

$$
\vec{v}(t)=(1+3t,\;-1+t)
$$

---

# 🔍 Step 3: Position

$$
\vec{r}(t)=\vec{r}_0+\vec{v}_0 t+\frac{1}{2}\vec{a}t^2
$$

---

### 🔄 Substitute:

$$
\vec{r}(t)=(0,0)+(t,-t)+\frac{1}{2}(3t^2,t^2)
$$

---

### 🔄 Simplify:

$$
\vec{r}(t)=\left(t+\frac{3}{2}t^2,\;-t+\frac{1}{2}t^2\right)
$$

---

### ✅ Result:

$$
\vec{r}(t)=\left(t+\frac{3}{2}t^2,\;-t+\frac{1}{2}t^2\right)
$$

---

# 🔍 Step 4: Trajectory

Eliminate $t$:

From:

$$
x=t+\frac{3}{2}t^2,\quad y=-t+\frac{1}{2}t^2
$$

This represents a **parabolic trajectory** in 2D.

---

# 🔍 Step 5: Work at $t=3$

### 🔄 Step 1: Find displacement

$$
\vec{r}(3)=\left(3+\frac{3}{2}\cdot9,\;-3+\frac{1}{2}\cdot9\right)
$$

$$
\vec{r}(3)=(3+13.5,\;-3+4.5)=(16.5,\;1.5)
$$

---

### 🔄 Step 2: Work

$$
W=\vec{F}\cdot\vec{r}
$$

$$
W=6\cdot16.5+2\cdot1.5
$$

$$
W=99+3=102\ \text{J}
$$

---

### ✅ Work:

$$
W=102\ \text{J}
$$

---

# 🔍 Step 6: Verify Work–Energy Theorem

### 🔄 Initial kinetic energy:

$$
K_0=\frac{1}{2}m v_0^2
$$

$$
v_0^2=1^2+(-1)^2=2
$$

$$
K_0=\frac{1}{2}\cdot2\cdot2=2\ \text{J}
$$

---

### 🔄 Final velocity at $t=3$:

$$
\vec{v}(3)=(1+9,\;-1+3)=(10,2)
$$

$$
v^2=10^2+2^2=104
$$

---

### 🔄 Final kinetic energy:

$$
K=\frac{1}{2}\cdot2\cdot104=104\ \text{J}
$$

---

### 🔄 Change in energy:

$$
\Delta K=104-2=102\ \text{J}
$$

---

### ✅ Verification:

$$
W=\Delta K=102\ \text{J}
$$

✔️ Work–energy theorem holds

---

# 🧩 Numerical Simulation (Python)

```python
import numpy as np
import matplotlib.pyplot as plt

t = np.linspace(0, 3, 100)

x = t + 1.5*t**2
y = -t + 0.5*t**2

plt.figure()
plt.plot(x, y)
plt.xlabel("x")
plt.ylabel("y")
plt.title("Trajectory")
plt.grid()
plt.show()