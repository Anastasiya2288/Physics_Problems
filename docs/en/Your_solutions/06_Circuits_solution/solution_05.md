# Kirchhoff’s Laws — Two-Loop Circuit

# Useful Definitions and Formulas

## 1. Electric Current

Electric current is the flow of electric charge through a conductor.

It is denoted by:

$$
I
$$

Unit:

$$
1A=1\frac{C}{s}
$$

---

# 2. Ohm’s Law

Ohm’s law describes the relationship between voltage, current, and resistance:

$$
U=IR
$$

where:

- $U$ — voltage
- $I$ — current
- $R$ — resistance

From this formula:

$$
I=\frac{U}{R}
$$

---

# 3. Kirchhoff’s First Law — Junction Rule

The algebraic sum of currents entering and leaving a junction is zero.

Mathematically:

$$
\sum I=0
$$

This means:

- currents entering a node equal currents leaving the node.

---

# 4. Kirchhoff’s Second Law — Loop Rule

The algebraic sum of voltages in any closed loop is zero.

Mathematically:

$$
\sum U=0
$$

When moving around a loop:

- voltage rise across a battery is positive,
- voltage drop across a resistor is negative.

---

# 5. Internal Resistance

Real batteries have internal resistance.

Voltage drop inside the battery:

$$
U_r=Ir
$$

where:

- $r$ — internal resistance

---

# Given Data

Left loop:

$$
R_1=20\Omega
$$

$$
\mathcal{E}_1=4.5V
$$

$$
r_1=1\Omega
$$

Shared branch:

$$
R_2=10\Omega
$$

Right loop:

$$
\mathcal{E}_2=9V
$$

$$
r_2=1\Omega
$$

Unknown currents:

$$
I_1,\ I_2,\ I_3
$$

---

# Step 1 — Apply Kirchhoff’s First Law

At the junction:

$$
I_3=I_1+I_2
$$

This means the current through the shared resistor equals the sum of currents from both loops.

---

# Step 2 — Left Loop Equation

Using Kirchhoff’s second law for the left loop:

$$
\mathcal{E}_1-I_1R_1-I_1r_1-I_3R_2=0
$$

Substitute values:

$$
4.5-20I_1-1I_1-10I_3=0
$$

Simplify:

$$
4.5-21I_1-10I_3=0
$$

Rearrange:

$$
21I_1+10I_3=4.5
$$

---

# Step 3 — Right Loop Equation

Apply Kirchhoff’s second law to the right loop:

$$
\mathcal{E}_2-I_2r_2-I_3R_2=0
$$

Substitute values:

$$
9-1I_2-10I_3=0
$$

Rearrange:

$$
I_2+10I_3=9
$$

---

# Step 4 — Use Junction Equation

From Kirchhoff’s first law:

$$
I_3=I_1+I_2
$$

Substitute into the previous equations.

---
## Equation 1

Substitute:

$$
I_3=I_1+I_2
$$

into:

$$
21I_1+10I_3=4.5
$$

We obtain:

$$
21I_1+10\left(I_1+I_2\right)=4.5
$$

Expand the brackets:

$$
21I_1+10I_1+10I_2=4.5
$$

Combine like terms:

$$
31I_1+10I_2=4.5
$$

---

## Equation 2

Substitute:

$$
I_3=I_1+I_2
$$

into:

$$
I_2+10I_3=9
$$

We obtain:

$$
I_2+10\left(I_1+I_2\right)=9
$$

Expand the brackets:

$$
I_2+10I_1+10I_2=9
$$

Combine like terms:

$$
10I_1+11I_2=9
$$
---

# Step 5 — Solve the System

We now solve:

$$
31I_1+10I_2=4.5
$$

$$
10I_1+11I_2=9
$$

---

## Eliminate $I_2$

Multiply the first equation by $11$:

$$
341I_1+110I_2=49.5
$$

Multiply the second equation by $10$:

$$
100I_1+110I_2=90
$$

Subtract equations:

$$
241I_1=-40.5
$$

$$
I_1=-0.168A
$$

---

# Step 6 — Find $I_2$

Substitute into:

$$
10I_1+11I_2=9
$$

$$
10$-0.168$+11I_2=9
$$

$$
-1.68+11I_2=9
$$

$$
11I_2=10.68
$$

$$
I_2=0.971A
$$

---

# Step 7 — Find $I_3$

Using:

$$
I_3=I_1+I_2
$$

$$
I_3=-0.168+0.971
$$

$$
I_3=0.803A
$$

---

# Final Answers

$$
\boxed{I_1=-0.168A}
$$

$$
\boxed{I_2=0.971A}
$$

$$
\boxed{I_3=0.803A}
$$

---

# Interpretation

The negative sign of $I_1$ means that the real direction of current $I_1$ is opposite to the initially assumed direction.