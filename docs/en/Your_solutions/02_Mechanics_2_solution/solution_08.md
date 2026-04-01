# 📘 Work of a Variable Force — Harmonic Oscillator

---

## 🔑 Key Definitions and Formulas

### 📌 Newton’s Second Law

$$
F=ma
$$

---

### 📌 Given Force (Hooke’s Law)

$$
F(x)=-kx
$$

This is a **restoring force** → always directed toward equilibrium.

---

### 📌 Work Done by a Variable Force

$$
W=\int_{x_1}^{x_2}F(x)\,dx
$$

---

### 📌 Potential Energy

$$
U(x)=-\int F(x)\,dx
$$

---

### 📌 Relation Between Force and Potential

$$
F=-\frac{dU}{dx}
$$

---

## 🧩 Part 1: Equation of Motion

### 🔄 Step 1: Apply Newton’s Second Law

$$
m\frac{d^2x}{dt^2}=-kx
$$

---

### 🔄 Step 2: Rearrange

$$
\frac{d^2x}{dt^2}+\frac{k}{m}x=0
$$

---

### 🔄 Step 3: Define Angular Frequency

$$
\omega=\sqrt{\frac{k}{m}}
$$

---

### 🔄 Step 4: General Solution

$$
x(t)=A\cos\left(\omega t\right)+B\sin\left(\omega t\right)
$$

---

### ✅ Interpretation:

This is **simple harmonic motion**.

---

## 🧩 Part 2: Work Done from $0$ to $x_0$

### 🔄 Step 1: Use definition

$$
W=\int_0^{x_0}-kx\,dx
$$

---

### 🔄 Step 2: Integrate

$$
W=-k\int_0^{x_0}x\,dx
$$

$$
W=-k\left[\frac{x^2}{2}\right]_0^{x_0}
$$

---

### 🔄 Step 3: Evaluate

$$
W=-\frac{kx_0^2}{2}
$$

---

### ✅ Result:

$$
W=-\frac{1}{2}kx_0^2
$$

---

## 🧩 Part 3: Potential Energy

From definition:

$$
U(x)=-\int F(x)\,dx
$$

---

### 🔄 Step 1: Substitute force

$$
U(x)=-\int(-kx)\,dx
$$

$$
U(x)=\int kx\,dx
$$

---

### 🔄 Step 2: Integrate

$$
U(x)=\frac{1}{2}kx^2
$$

---

### ✅ Result:

$$
U(x)=\frac{1}{2}kx^2
$$

---

### 🧠 Interpretation:

- Energy increases with displacement
- Minimum at $x=0$
- This is a **parabolic potential well**

---

## 🧩 Part 4: Verify $F=-\frac{dU}{dx}$

### 🔄 Step 1: Differentiate

$$
\frac{dU}{dx}=\frac{d}{dx}\left(\frac{1}{2}kx^2\right)
$$

$$
\frac{dU}{dx}=kx
$$

---

### 🔄 Step 2: Add minus sign

$$
F=-\frac{dU}{dx}=-kx
$$

---

### ✅ Verified ✔️

---

## 🧩 Part 5: Graph Interpretation

### 📌 Force $F(x)$:

$$
F(x)=-kx
$$

- Straight line
- Passes through origin
- Negative slope

---

### 📌 Potential Energy $U(x)$:

$$
U(x)=\frac{1}{2}kx^2
$$

- Parabola
- Minimum at $x=0$
- Always positive

---

## 🎯 Final Summary

- Motion is **simple harmonic**
- Work done:
  
$$
W=-\frac{1}{2}kx_0^2
$$

- Potential energy:

$$
U(x)=\frac{1}{2}kx^2
$$

- Force–energy relation verified:

$$
F=-\frac{dU}{dx}
$$

---