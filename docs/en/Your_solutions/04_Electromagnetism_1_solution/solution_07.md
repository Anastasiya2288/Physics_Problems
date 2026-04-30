## 7. Cyclotron Motion

---

### Useful Definitions and Formulas

- **Work-energy theorem** (acceleration through potential difference $U$):
$$eU = \frac{1}{2}m_e v^2$$

- **Lorentz magnetic force** (provides centripetal acceleration):
$$F = evB$$

- **Centripetal force condition:**
$$evB = \frac{m_e v^2}{r}$$

- **Radius of circular motion:**
$$r = \frac{m_e v}{eB}$$

- **Combining** (eliminating $v$):
$$r = \frac{\sqrt{2m_e eU}}{eB} = \frac{1}{B}\sqrt{\frac{2m_e U}{e}}$$

**Constants:**
| Quantity | Symbol | Value |
|---|---|---|
| Electron mass | $m_e$ | $9.109 \times 10^{-31}\ \text{kg}$ |
| Elementary charge | $e$ | $1.602 \times 10^{-19}\ \text{C}$ |

---

### Step-by-Step Solution

**Step 1: Find the electron's velocity after acceleration.**

The potential difference $U$ converts electrical potential energy into kinetic energy:

$$eU = \frac{1}{2}m_e v^2 \implies v = \sqrt{\frac{2eU}{m_e}}$$

Substituting values:

$$v = \sqrt{\frac{2 \times (1.602\times10^{-19}) \times 5000}{9.109\times10^{-31}}}$$

$$v = \sqrt{\frac{1.602\times10^{-15}}{9.109\times10^{-31}}} = \sqrt{1.759\times10^{15}} \approx 4.195\times10^7\ \text{m/s}$$

> **Note:** $v/c \approx 0.14$, so relativistic effects are small but present — we proceed classically as a good approximation.

---

**Step 2: Apply the circular motion condition.**

The magnetic force acts perpendicular to $v$ at all times, curving the path into a circle. Setting magnetic force equal to centripetal force:

$$evB = \frac{m_e v^2}{r} \implies r = \frac{m_e v}{eB}$$

---

**Step 3: Substitute numerical values.**

$$r = \frac{m_e v}{eB} = \frac{9.109\times10^{-31} \times 4.195\times10^7}{1.602\times10^{-19} \times 0.1}$$

**Numerator:**
$$9.109\times10^{-31} \times 4.195\times10^7 = 3.821\times10^{-23}\ \text{kg·m/s}$$

**Denominator:**
$$1.602\times10^{-19} \times 0.1 = 1.602\times10^{-20}\ \text{C·T}$$

$$r = \frac{3.821\times10^{-23}}{1.602\times10^{-20}} \approx 2.385\times10^{-3}\ \text{m}$$

---

**Step 4 (Alternative): Use the combined formula directly.**

$$r = \frac{1}{B}\sqrt{\frac{2m_e U}{e}} = \frac{1}{0.1}\sqrt{\frac{2 \times 9.109\times10^{-31} \times 5000}{1.602\times10^{-19}}}$$

$$= 10 \times \sqrt{\frac{9.109\times10^{-27}}{1.602\times10^{-19}}} = 10 \times \sqrt{5.686\times10^{-8}}$$

$$= 10 \times 2.385\times10^{-4} \approx 2.385\times10^{-3}\ \text{m}$$

---

### Result

$$\boxed{r \approx 2.39\ \text{mm}}$$

> **Physical interpretation:** The electron moves in a tight circle of radius ~2.4 mm. The radius is small because:
> - The electron is very light ($m_e$ is tiny), so even moderate speeds