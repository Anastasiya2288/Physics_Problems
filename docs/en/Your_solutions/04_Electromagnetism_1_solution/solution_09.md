## 9. Vector Lorentz Force

---

### Useful Definitions and Formulas

- **Magnetic Lorentz force:**
$$\vec{F} = q\vec{v} \times \vec{B}$$

- **Cross product** of two vectors $\vec{A} = (A_x, A_y, A_z)$ and $\vec{B} = (B_x, B_y, B_z)$:
$$\vec{A} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ A_x & A_y & A_z \\ B_x & B_y & B_z \end{vmatrix}$$

$$= \hat{i}(A_y B_z - A_z B_y) - \hat{j}(A_x B_z - A_z B_x) + \hat{k}(A_x B_y - A_y B_x)$$

- **Magnitude of a vector** $\vec{F} = (F_x, F_y, F_z)$:
$$|\vec{F}| = \sqrt{F_x^2 + F_y^2 + F_z^2}$$

- **Proton charge:**
$$q_p = e = 1.602\times10^{-19}\ \text{C}$$

---

### Setup

$$\vec{v} = (2,\ -4,\ 1)\ \text{m/s}, \qquad \vec{B} = (1,\ 2,\ -1)\ \text{T}$$

---

### Step-by-Step Solution

**Step 1: Compute the cross product $\vec{v} \times \vec{B}$.**

$$\vec{v} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & -4 & 1 \\ 1 & 2 & -1 \end{vmatrix}$$

Expand along the first row:

**$\hat{i}$ component:**
$$\hat{i}\left[(-4)(-1) - (1)(2)\right] = \hat{i}\left[4 - 2\right] = 2\hat{i}$$

**$\hat{j}$ component** (note the minus sign):
$$-\hat{j}\left[(2)(-1) - (1)(1)\right] = -\hat{j}\left[-2 - 1\right] = -\hat{j}(-3) = 3\hat{j}$$

**$\hat{k}$ component:**
$$\hat{k}\left[(2)(2) - (-4)(1)\right] = \hat{k}\left[4 + 4\right] = 8\hat{k}$$

Therefore:
$$\vec{v} \times \vec{B} = (2,\ 3,\ 8)\ \text{m/s} \cdot \text{T}$$

---

**Step 2: Verify with the full determinant check.**

| Component | Formula | Calculation | Result |
|-----------|---------|-------------|--------|
| $i$ | $v_y B_z - v_z B_y$ | $(-4)(-1)-(1)(2)$ | $+2$ |
| $j$ | $v_z B_x - v_x B_z$ | $(1)(1)-(2)(-1)$ | $+3$ |
| $k$ | $v_x B_y - v_y B_x$ | $(2)(2)-(-4)(1)$ | $+8$ |

Confirmed: $\vec{v} \times \vec{B} = 2\hat{i} + 3\hat{j} + 8\hat{k}$

---

**Step 3: Multiply by the proton charge.**

$$\vec{F} = q(\vec{v} \times \vec{B}) = e\,(2\hat{i} + 3\hat{j} + 8\hat{k})$$

$$\vec{F} = 1.602\times10^{-19} \times (2\hat{i} + 3\hat{j} + 8\hat{k})$$

$$\vec{F} = (3.204\hat{i} + 4.806\hat{j} + 12.816\hat{k})\times10^{-19}\ \text{N}$$

---

**Step 4: Compute the magnitude of $\vec{v} \times \vec{B}$ first.**

$$|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2} = \sqrt{4 + 9 + 64} = \sqrt{77}\ \text{m/s} \cdot \text{T}$$

$$\sqrt{77} \approx 8.775\ \text{m/s} \cdot \text{T}$$

---

**Step 5: Compute the magnitude of the force.**

$$|\vec{F}| = e\,|\vec{v} \times \vec{B}| = 1.602\times10^{-19} \times \sqrt{77}$$

$$|\vec{F}| = 1.602\times10^{-19} \times 8.775 \approx 1.406\times10^{-18}\ \text{N}$$

---

### Result

$$\boxed{\vec{F} = e\,(2\hat{i} + 3\hat{j} + 8\hat{k})\ \text{N} \approx (3.20\hat{i} + 4.81\hat{j} + 12.82\hat{k})\times10^{-19}\ \text{N}}$$

$$\boxed{|\vec{F}| = e\sqrt{77} \approx 1.406\times10^{-18}\ \text{N}}$$

> **Physical notes:**
> - The force vector $(2, 3, 8)$ is perpendicular to both $\vec{v}$ and $\vec{B}$ — you can verify: $(2,3,8)\cdot(2,-4,1) = 4-12+8 = 0$ ✓ and $(2,3,8)\cdot(1,2,-1) = 2+6-8 = 0$ ✓
> - The magnetic force does **no work**: it is always perpendicular to the velocity.
> - The dominant component is along $\hat{k}$, since the $\hat{k}$ contributions from the cross product are largest.