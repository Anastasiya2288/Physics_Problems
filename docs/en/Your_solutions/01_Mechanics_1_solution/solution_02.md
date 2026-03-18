# Range Optimization — Theory + Analytical Proof

---

# Useful Definitions and Formulas

### 1. Range of Projectile Motion

For motion without air resistance, the horizontal range is:

$$
R(\theta)=\frac{v_0^2\sin2\theta}{g}
$$

where:
- $v_0$ — initial velocity
- $\theta$ — launch angle
- $g$ — gravitational acceleration

---

### 2. Optimization Principle

To find the **maximum value** of a function $R(\theta)$:

- Take the derivative:
$$
\frac{dR}{d\theta}
$$

- Set it equal to zero:
$$
\frac{dR}{d\theta}=0
$$

- Solve for $\theta$

---

### 3. Derivative of Trigonometric Function

$$
\frac{d}{d\theta}\sin2\theta=2\cos2\theta
$$

---

# Step-by-Step Solution

We are given:

$$
R(\theta)=\frac{v_0^2\sin2\theta}{g}
$$

---

# Step 1. Simplify the Expression

Since $\frac{v_0^2}{g}$ is constant, denote:

$$
R(\theta)=C\sin2\theta
$$

where:

$$
C=\frac{v_0^2}{g}
$$

---

# Step 2. Differentiate the Range Function

$$
\frac{dR}{d\theta}=C\cdot2\cos2\theta
$$

$$
\frac{dR}{d\theta}=\frac{2v_0^2}{g}\cos2\theta
$$

---

# Step 3. Find Critical Points

Set derivative equal to zero:

$$
\frac{2v_0^2}{g}\cos2\theta=0
$$

Since $\frac{2v_0^2}{g}\neq0$, we get:

$$
\cos2\theta=0
$$

---

# Step 4. Solve the Equation

$$
2\theta=\frac{\pi}{2}
$$

$$
\theta=\frac{\pi}{4}
$$

---

# Step 5. Convert to Degrees

$$
\theta=45^\circ
$$

---

# Step 6. Verify Maximum

Second derivative:

$$
\frac{d^2R}{d\theta^2}=-\frac{4v_0^2}{g}\sin2\theta
$$

At $\theta=45^\circ$:

$$
\sin2\theta=\sin90^\circ=1
$$

Thus:

$$
\frac{d^2R}{d\theta^2}<0
$$

So this point is a **maximum**.

---

# Final Answer

$$
\theta_{\text{max}}=45^\circ
$$

---

# Key Insight

- The range depends on $\sin2\theta$
- The maximum value of $\sin x$ is $1$
- This happens when:

$$
2\theta=90^\circ
$$

$$
\theta=45^\circ
$$

---

# Conclusion

The projectile achieves **maximum range at $45^\circ$** because this angle maximizes the sine function in the range formula.