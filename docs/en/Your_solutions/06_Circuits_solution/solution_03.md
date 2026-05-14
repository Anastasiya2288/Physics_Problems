# Mixed Circuit — Equivalent Resistance
![alt text](../../image-r1.png)
## Useful Definitions and Formulas

### 1. Equivalent Resistance

Equivalent resistance is the single resistance that can replace the entire circuit without changing the total current supplied by the source.

It is denoted as:

$$
R_{eq}
$$

---

## 2. Series Connection

Resistors are connected in series when the same current flows through all of them.

For resistors in series:

$$
R_{eq}=R_1+R_2+R_3+\dots
$$

Important property:

- Current is the same through all resistors.
- Total resistance increases.

---

## 3. Parallel Connection

Resistors are connected in parallel when they share the same two nodes.

For resistors in parallel:

$$
\frac{1}{R_{eq}}=\frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}+\dots
$$

For two equal resistors:

$$
R_{eq}=\frac{R}{2}
$$

Important property:

- Voltage is the same across all branches.
- Total resistance decreases.

---

# Step-by-Step Solution

All resistors have resistance:

$$
R=5\Omega
$$

The circuit is a mixed circuit, which means it contains both series and parallel connections.

---

## Step 1 — Identify Parallel Resistors

Suppose two resistors are connected in parallel.

Since both resistors are equal:

$$
R_p=\frac{R\cdot R}{R+R}
$$

Substitute the values:

$$
R_p=\frac{5\cdot5}{5+5}
$$

$$
R_p=\frac{25}{10}
$$

$$
R_p=2.5\Omega
$$

So the equivalent resistance of the parallel part is:

$$
R_p=2.5\Omega
$$

---

## Step 2 — Add Series Resistors

Now this equivalent resistance is connected in series with another resistor of $5\Omega$.

For series connection:

$$
R_{eq}=R_s+R_p
$$

Substitute values:

$$
R_{eq}=5+2.5
$$

$$
R_{eq}=7.5\Omega
$$

---

# Final Answer

The equivalent resistance of the circuit is:

$$
\boxed{R_{eq}=7.5\Omega}
$$