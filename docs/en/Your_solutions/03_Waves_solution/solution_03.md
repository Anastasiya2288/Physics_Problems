# 3. Superposition Principle

## 📘 Key Definitions and Formulas

### 1. Principle of Superposition
When two waves overlap, the resulting displacement is the **sum** of the individual displacements:

$$y(x,t)=y_1(x,t)+y_2(x,t)$$

---

### 2. Given Wave Equations

$$y_1(x,t)=A\sin(kx-\omega t)$$  
$$y_2(x,t)=A\sin(kx+\omega t)$$

These represent two waves with:
- Same amplitude $A$
- Same wave number $k$
- Same angular frequency $\omega$
- Moving in **opposite directions**

---

### 3. Trigonometric Identity

To combine the waves, we use:

$$\sin\alpha+\sin\beta=2\sin\frac{\alpha+\beta}{2}\cos\frac{\alpha-\beta}{2}$$

---

## 🧮 Step-by-Step Solution

## 🔹 Step 1: Apply Superposition

$$y(x,t)=A\sin(kx-\omega t)+A\sin(kx+\omega t)$$

Factor out $A$:

$$y(x,t)=A[\sin(kx-\omega t)+\sin(kx+\omega t)]$$

---

## 🔹 Step 2: Apply Trigonometric Identity

Let:
- $\alpha=kx-\omega t$
- $\beta=kx+\omega t$

Then:

$$y(x,t)=2A\sin\frac{(kx-\omega t)+(kx+\omega t)}{2}\cos\frac{(kx-\omega t)-(kx+\omega t)}{2}$$

---

## 🔹 Step 3: Simplify Expressions

### First term:

$$\frac{(kx-\omega t)+(kx+\omega t)}{2}=\frac{2kx}{2}=kx$$

### Second term:

$$\frac{(kx-\omega t)-(kx+\omega t)}{2}=\frac{-2\omega t}{2}=-\omega t$$

---

## 🔹 Step 4: Final Equation

$$y(x,t)=2A\sin(kx)\cos(\omega t)$$

---

## 🎯 Resulting Standing Wave

$$y(x,t)=2A\sin(kx)\cos(\omega t)$$

✔️ This is a **standing wave**:
- $\sin(kx)$ → spatial part
- $\cos(\omega t)$ → time oscillation

---

## 📍 Step 5: Positions of Nodes

### Definition of Nodes
Nodes are points where displacement is always zero:

$$y(x,t)=0\quad\text{for all }t$$

This happens when:

$$\sin(kx)=0$$

---

### Solve for Node Positions

$$kx=n\pi,\quad n=0,\pm1,\pm2,\dots$$

Solve for $x$:

$$x=\frac{n\pi}{k}$$

---

### Using $k=\frac{2\pi}{\lambda}$

$$x=\frac{n\pi}{2\pi/\lambda}=\frac{n\lambda}{2}$$

---

## 🎯 Final Answer

### Standing wave equation:
$$y(x,t)=2A\sin(kx)\cos(\omega t)$$

### Node positions:
$$x=\frac{n\lambda}{2},\quad n=0,\pm1,\pm2,\dots$$

---

## 💡 Final Insight

✔️ The wave is stationary because energy does not propagate — it oscillates in place.  
✔️ Nodes are fixed points with zero motion.  
✔️ The distance between adjacent nodes is $\frac{\lambda}{2}$.