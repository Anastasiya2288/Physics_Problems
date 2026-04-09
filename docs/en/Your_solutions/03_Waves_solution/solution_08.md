# 8. Waves

## 📘 Key Definitions and Formulas

### 1. Wave Equation

A function describes a traveling wave if it satisfies:

$$\frac{\partial^2 y}{\partial x^2}=\frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}$$

---

### 2. General Form of Traveling Wave

Any function of the form:

$$y(x,t)=f(x\pm vt)$$

is a valid traveling wave solution.

✔️ This is the **most important shortcut**.

---

## 🧮 Step-by-Step Analysis

---

## 🔹 a) $y(x,t)=A\cos(kx^2-\omega t)$

### ❌ Check structure:
- Inside cosine: $kx^2-\omega t$
- This is **not** of the form $x\pm vt$

### ❌ Conclusion:
This function does **not** represent a traveling wave.

---

## 🔹 b) $y(x,t)=A(x-vt)^2$

### ✔️ Check structure:
- Depends on $(x-vt)$

This matches:

$$y(x,t)=f(x-vt)$$

### ✔️ Conclusion:
This **is a valid traveling wave**.

---

## 🔹 c) $y(x,t)=A\log(x+vt)$

### ✔️ Check structure:
- Depends on $(x+vt)$

This matches:

$$y(x,t)=f(x+vt)$$

### ✔️ Conclusion:
This **is a valid traveling wave**.

---

## 🎯 Final Answer

- a) ❌ Not a traveling wave  
- b) ✔️ Traveling wave  
- c) ✔️ Traveling wave  

---

## 💡 Final Insight

✔️ The fastest way to check is to see if the function depends only on $x\pm vt$.  
✔️ If yes → automatically satisfies the wave equation.  
✔️ If not → it is not a pure traveling wave.