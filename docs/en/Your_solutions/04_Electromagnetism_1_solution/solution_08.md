## 8. Lorentz Force

---

### Useful Definitions and Formulas

- **General Lorentz force** (electric + magnetic):
$$\vec{F} = q(\vec{E} + \vec{v} \times \vec{B})$$

- **Magnetic Lorentz force only** (no electric field):
$$\vec{F} = q\vec{v} \times \vec{B}$$

- **Magnitude** (when $\vec{v} \perp \vec{B}$, i.e. $\sin\theta = 1$):
$$F = qvB$$

- **General magnitude** for arbitrary angle $\theta$ between $\vec{v}$ and $\vec{B}$:
$$F = qvB\sin\theta$$

- **Direction:** perpendicular to both $\vec{v}$ and $\vec{B}$, given by the right-hand rule.

- **Radius of resulting circular orbit:**
$$r = \frac{mv}{qB}$$

- **Cyclotron (angular) frequency:**
$$\omega = \frac{qB}{m}$$

---

### Step-by-Step Solution

**Step 1: Identify the geometry.**

The particle enters **perpendicular** to the field, meaning the angle between $\vec{v}$ and $\vec{B}$ is:
$$\theta = 90° \implies \sin\theta = 1$$

This is the maximum possible force configuration — the full speed contributes to the force.

---

**Step 2: Write the force formula.**

Since $\vec{v} \perp \vec{B}$:

$$F = qvB$$

---

**Step 3: Substitute the given values.**

$$F = q \cdot v \cdot B = (2\times10^{-19}\ \text{C}) \times (10^6\ \text{m/s}) \times (0.5\ \text{T})$$

---

**Step 4: Compute step by step.**

First multiply $q \cdot v$:
$$2\times10^{-19} \times 10^6 = 2\times10^{-13}\ \text{C} \cdot \text{m/s}$$

Then multiply by $B$:
$$F = 2\times10^{-13} \times 0.5 = 1\times10^{-13}\ \text{N}$$

---

**Step 5: Bonus — find the orbital radius.**

Since the magnetic force acts as centripetal force, we can also find the radius of curvature:

$$r = \frac{mv}{qB} = \frac{(4\times10^{-27}) \times (10^6)}{(2\times10^{-19}) \times (0.5)}$$

$$r = \frac{4\times10^{-21}}{1\times10^{-19}} = 4\times10^{-2}\ \text{m} = 4\ \text{cm}$$

And the cyclotron frequency:

$$\omega = \frac{qB}{m} = \frac{(2\times10^{-19}) \times (0.5)}{4\times10^{-27}} = \frac{10^{-19}}{4\times10^{-27}} = 2.5\times10^{7}\ \text{rad/s}$$

---

### Result

$$\boxed{F = qvB = 1\times10^{-13}\ \text{N} = 0.1\ \text{pN}}$$

> **Physical interpretation:**
> - The force $F = 0.1\ \text{pN}$ is tiny by everyday standards, yet it is enormous relative to the particle's weight ($mg \approx 3.9\times10^{-26}\ \text{N}$) — the Lorentz force exceeds gravity by a factor of $\sim 10^{12}$.
> - The magnetic force **does no work** on the particle (always perpendicular to $\vec{v}$), so the speed remains constant — only the direction changes.
> - The particle traces a **circle** of radius $r = 4\ \text{cm}$ in the plane perpendicular to $\vec{B}$.