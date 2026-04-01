# 📘 Vertical Throw with Linear Drag

---

## 🔑 Key Definitions and Formulas

### 📌 Equation of Motion

$$
m\frac{dv}{dt}=-mg-kv
$$

This includes:
- gravity $-mg$
- linear drag $-kv$

---

### 📌 Standard First-Order Linear ODE

$$
\frac{dv}{dt}+a v=b
$$

Solution:

$$
v(t)=C e^{-at}+\frac{b}{a}
$$

---

### 📌 Relation Between Velocity and Position

$$
v=\frac{dx}{dt}
$$

---

## 🧩 Part 1: Solve the Differential Equation

### 🔄 Step 1: Rewrite equation

Divide by $m$:

$$
\frac{dv}{dt}+\frac{k}{m}v=-g
$$

---

### 🔄 Step 2: Define constant

$$
\gamma=\frac{k}{m}
$$

So:

$$
\frac{dv}{dt}+\gamma v=-g
$$

---

### 🔄 Step 3: Solve equation

General solution:

$$
v(t)=C e^{-\gamma t}-\frac{g}{\gamma}
$$

---

### 🔄 Step 4: Apply initial condition $v(0)=v_0$

$$
v_0=C-\frac{g}{\gamma}
$$

$$
C=v_0+\frac{g}{\gamma}
$$

---

### ✅ Final velocity:

$$
v(t)=\left(v_0+\frac{g}{\gamma}\right)e^{-\gamma t}-\frac{g}{\gamma}
$$

---

## 🧩 Part 2: Position Function

### 🔄 Step 1: Integrate velocity

$$
x(t)=\int v(t)\,dt
$$

---

### 🔄 Step 2: Integrate term by term

$$
x(t)=\left(v_0+\frac{g}{\gamma}\right)\frac{-1}{\gamma}e^{-\gamma t}-\frac{g}{\gamma}t+C
$$

---

### 🔄 Step 3: Apply $x(0)=10$

$$
10=-\frac{1}{\gamma}\left(v_0+\frac{g}{\gamma}\right)+C
$$

$$
C=10+\frac{1}{\gamma}\left(v_0+\frac{g}{\gamma}\right)
$$

---

### ✅ Final position:

$$
x(t)=10+\frac{1}{\gamma}\left(v_0+\frac{g}{\gamma}\right)\left(1-e^{-\gamma t}\right)-\frac{g}{\gamma}t
$$

---

## 🧩 Part 3: Maximum Height

At maximum height:

$$
v(t_{\max})=0
$$

---

### 🔄 Step 1: Solve for $t_{\max}$

$$
0=\left(v_0+\frac{g}{\gamma}\right)e^{-\gamma t}-\frac{g}{\gamma}
$$

$$
e^{-\gamma t}=\frac{g}{\gamma v_0+g}
$$

---

### 🔄 Step 2: Solve for time

$$
t_{\max}=\frac{1}{\gamma}\ln\left(\frac{\gamma v_0+g}{g}\right)
$$

---

### 🔄 Step 3: Substitute into $x(t)$

Maximum height:

$$
x_{\max}=x(t_{\max})
$$

(analytical expression is long, but computable)

---

## 🧩 Part 4: Comparison Without Drag

Without drag:

$$
v(t)=v_0-gt
$$

Maximum height:

$$
h=\frac{v_0^2}{2g}
$$

---

### 🧠 Conclusion:

- With drag → **lower height**
- With drag → velocity decreases faster
- Motion becomes asymmetric

---

## 🧩 Part 5: Numerical Simulation (Python)

```python
import numpy as np
import matplotlib.pyplot as plt

# parameters
m = 1.0
k = 0.5
g = 9.81
v0 = 20
x0 = 10

gamma = k/m

# time array
t = np.linspace(0, 5, 500)

# velocity
v = (v0 + g/gamma)*np.exp(-gamma*t) - g/gamma

# position
x = x0 + (v0 + g/gamma)/gamma*(1 - np.exp(-gamma*t)) - (g/gamma)*t

# plot
plt.figure()
plt.plot(t, x, label="Position x(t)")
plt.plot(t, v, label="Velocity v(t)")
plt.xlabel("Time")
plt.legend()
plt.grid()
plt.show()


