## 6. Field at a Point from a System of Charges

---

### Useful Definitions and Formulas

- **Electric field** from a point charge $Q$ at distance $r$:
$$\vec{E} = \frac{1}{4\pi\varepsilon_0}\frac{Q}{r^2}\hat{r}$$

- **Superposition principle:** The total field is the vector sum of individual fields:
$$\vec{E} = \vec{E}_1 + \vec{E}_2$$

- **Coulomb constant:**
$$k = \frac{1}{4\pi\varepsilon_0} \approx 8.99 \times 10^9\ \text{N} \cdot \text{m}^2/\text{C}^2$$

- **Component form:** If charge $Q$ is at position $\vec{r}_0$ and field point is $\vec{r}$:
$$\vec{E} = k\frac{Q}{|\vec{r}-\vec{r}_0|^3}(\vec{r}-\vec{r}_0)$$

---

### Setup

| Charge | Position | Value |
|--------|----------|-------|
| $q_1$ | $(-a,\ 0)$ | $+q$ |
| $q_2$ | $(a,\ 0)$ | $+2q$ |

Field point: $P = (x,\ y)$

**Displacement vectors from each charge to point $P$:**

$$\vec{r}_1 = (x+a,\ y), \quad r_1 = \sqrt{(x+a)^2 + y^2}$$

$$\vec{r}_2 = (x-a,\ y), \quad r_2 = \sqrt{(x-a)^2 + y^2}$$

---

## Part 1 — Electric Field Vectors

### General Field $\vec{E}(x,y)$

By superposition:

$$\boxed{\vec{E}(x,y) = kq\frac{(x+a,\ y)}{[(x+a)^2+y^2]^{3/2}} + 2kq\frac{(x-a,\ y)}{[(x-a)^2+y^2]^{3/2}}}$$

In components:

$$E_x(x,y) = kq\left[\frac{x+a}{[(x+a)^2+y^2]^{3/2}} + \frac{2(x-a)}{[(x-a)^2+y^2]^{3/2}}\right]$$

$$E_y(x,y) = kqy\left[\frac{1}{[(x+a)^2+y^2]^{3/2}} + \frac{2}{[(x-a)^2+y^2]^{3/2}}\right]$$

---

### Field on the $y$-axis: $\vec{E}(0,y)$

Set $x = 0$. The displacement vectors become $(\pm a,\ y)$ with equal magnitude $r = \sqrt{a^2+y^2}$.

**$x$-components** from charge $+q$: contributes $-a$ direction; from $+2q$: contributes $+a$ direction.

$$E_x(0,y) = \frac{kq}{(a^2+y^2)^{3/2}}\left[-a + 2a\right] = \frac{kqa}{(a^2+y^2)^{3/2}}$$

> The $x$-components do **not** cancel because the charges are unequal!

**$y$-components** both point in $+y$ (both charges positive):

$$E_y(0,y) = \frac{kqy}{(a^2+y^2)^{3/2}}\left[1 + 2\right] = \frac{3kqy}{(a^2+y^2)^{3/2}}$$

$$\boxed{\vec{E}(0,y) = \frac{kq}{(a^2+y^2)^{3/2}}\left(a,\ 3y\right)}$$

---

### Field on the $x$-axis: $\vec{E}(x,0)$

Set $y = 0$. Both fields point purely along $x$-axis (charges lie on $x$-axis).

$$\vec{E}(x,0) = kq\frac{\hat{x}_1}{(x+a)^2} + 2kq\frac{\hat{x}_2}{(x-a)^2}$$

where $\hat{x}_1 = \text{sign}(x+a)$ and $\hat{x}_2 = \text{sign}(x-a)$.

For the region $x > a$ (both fields in $+x$):

$$\boxed{E_x(x,0) = kq\left[\frac{1}{(x+a)^2} + \frac{2}{(x-a)^2}\right], \quad E_y = 0}$$

---

## Part 2 — Conditions for Zero Components

### Condition $E_y = 0$

From the general formula, $E_y \propto y\left[\frac{1}{r_1^3} + \frac{2}{r_2^3}\right]$.

Since both terms in the bracket are always positive, $E_y = 0$ **only when $y = 0$**, i.e., on the $x$-axis.

$$\boxed{E_y = 0 \iff y = 0}$$

### Condition $E_x = 0$

On the $x$-axis ($y=0$), we need:

$$\frac{1}{(x+a)^2} + \frac{2}{(x-a)^2} = 0$$

This has **no real solution** for $x > a$ or $x < -a$ (both terms positive).

For $-a < x < a$, the signs differ:

$$\frac{1}{(x+a)^2} = \frac{2}{(x-a)^2}$$

$$(x-a)^2 = 2(x+a)^2$$

$$|x-a| = \sqrt{2}|x+a|$$

Taking the case where $x-a < 0$ and $x+a > 0$ (i.e., $-a < x < a$):

$$-(x-a) = \sqrt{2}(x+a)$$

$$a - x = \sqrt{2}\,x + \sqrt{2}\,a$$

$$a(1-\sqrt{2}) = x(1+\sqrt{2})$$

$$\boxed{x_0 = \frac{a(1-\sqrt{2})}{1+\sqrt{2}} = a(1-\sqrt{2})\frac{(1-\sqrt{2})}{(1-2)} = a(\sqrt{2}-1)^2 \cdot (-1)}$$

Let's simplify cleanly:

$$x_0 = a\cdot\frac{1-\sqrt{2}}{1+\sqrt{2}} = a\cdot\frac{(1-\sqrt{2})^2}{1-2} = a({\sqrt{2}-1})^2$$

$$\boxed{x_0 = a(3 - 2\sqrt{2}) \approx -0.172\,a}$$

> This point lies between the two charges, closer to the stronger charge $+2q$.

### Condition $\vec{E} = 0$ (zero total field)

Since $E_y = 0$ requires $y=0$, the zero-field point must lie on the $x$-axis.
On the $x$-axis the field is purely in $x$, so we need $E_x = 0$ as found above.

$$\boxed{\vec{E} = 0 \text{ at } (x_0,\ 0) = \left(a(3-2\sqrt{2}),\ 0\right) \approx (-0.172\,a,\ 0)}$$

> **Physical intuition:** The weaker charge $+q$ (on the left) and the stronger $+2q$ (on the right) create a null point