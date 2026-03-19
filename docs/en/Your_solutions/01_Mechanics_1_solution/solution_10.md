# Kinematics — Theory + Solution

---

# Useful Definitions and Formulas

### 1. Parametric Curve

A trajectory in space is given by:

$$
\vec{r}(t)=(x(t),y(t),z(t))
$$

---

### 2. Eliminating Parameter

To find the trajectory:
- eliminate $t$ between coordinates

---

### 3. Arc Length (Path Length)

The length of a curve is:

$$
S=\int_{0}^{t_0}|\vec{v}(t)|dt
$$

where:

$$
\vec{v}(t)=\frac{d\vec{r}}{dt}
$$

---

### 4. Speed

$$
|\vec{v}(t)|=\sqrt{\left(\frac{dx}{dt}\right)^2+\left(\frac{dy}{dt}\right)^2+\left(\frac{dz}{dt}\right)^2}
$$

---

# Step-by-Step Solution

Given:

$$
\vec{r}(t)=(a\cos(\omega t),\ b\sin(\omega t),\ bt)
$$

---

# a) Trajectory Equation

From coordinates:

$$
x=a\cos(\omega t),\quad y=b\sin(\omega t)
$$

Divide:

$$
\frac{x}{a}=\cos(\omega t),\quad \frac{y}{b}=\sin(\omega t)
$$

---

Square and add:

$$
\left(\frac{x}{a}\right)^2+\left(\frac{y}{b}\right)^2=1
$$

---

### Result:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

---

For $z$:

$$
z=bt \Rightarrow t=\frac{z}{b}
$$

---

### Final trajectory:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1,\quad z=\frac{b}{\omega}\arctan\left(\frac{y}{x}\right)\ \text{(implicit helical form)}
$$

---

### Interpretation

- Projection on $xy$ plane → ellipse  
- Along $z$ → linear motion  

➡️ This is an **elliptical helix**

---

# b) Path Length

---

# Step 1. Velocity

Differentiate:

$$
\frac{dx}{dt}=-a\omega\sin(\omega t)
$$

$$
\frac{dy}{dt}=b\omega\cos(\omega t)
$$

$$
\frac{dz}{dt}=b
$$

---

### Velocity vector:

$$
\vec{v}(t)=(-a\omega\sin(\omega t),\ b\omega\cos(\omega t),\ b)
$$

---

# Step 2. Speed

$$
|\vec{v}(t)|=\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}
$$

---

Factor:

$$
|\vec{v}(t)|=\sqrt{\omega^2(a^2\sin^2(\omega t)+b^2\cos^2(\omega t))+b^2}
$$

---

# Step 3. Path Length

$$
S=\int_0^{t_0}\sqrt{\omega^2(a^2\sin^2(\omega t)+b^2\cos^2(\omega t))+b^2}\ dt
$$

---

### Special simplification (important case):

If $a=b$:

$$
|\vec{v}(t)|=\sqrt{a^2\omega^2+b^2}
$$

(constant)

---

Then:

$$
S=\sqrt{a^2\omega^2+b^2}\cdot t_0
$$

---

# c) Python Visualization

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
a = 2
b = 1
omega = 1
t = np.linspace(0, 10, 1000)

# Parametric equations
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

# Plot
fig = plt.figure()
ax = fig.add_subplot(projection='3d')

ax.plot(x, y, z)
ax.set_xlabel('X')
ax.set_ylabel('Y')
ax.set_zlabel('Z')

plt.show()