# Mixed Circuit — Equivalent Resistance
![alt text](../../image-r2.png)
## Useful Definitions and Formulas

### 1. Equivalent Resistance

Equivalent resistance is the total resistance of the whole circuit seen by the power source.

It is written as:

$$
R_{eq}
$$

The purpose of finding equivalent resistance is to replace a complicated circuit with one single resistor.

---

## 2. Series Connection

Resistors are connected in series when current flows through them one after another in a single path.

For resistors in series:

$$
R_{eq}=R_1+R_2+R_3+\dots
$$

Important properties:

- The same current flows through all resistors.
- Total resistance increases.

---

## 3. Parallel Connection

Resistors are connected in parallel when both ends of the resistors are connected to the same two nodes.

For resistors in parallel:

$$
\frac{1}{R_{eq}}=\frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}+\dots
$$

For two equal resistors:

$$
R_{eq}=\frac{R}{2}
$$

Important properties:

- Voltage is the same across each branch.
- Equivalent resistance becomes smaller than the smallest resistor.

---

# Step-by-Step Solution

All resistors have resistance:

$$
R=10\Omega
$$

The circuit is a mixed circuit, meaning it contains both series and parallel resistor connections.

---

## Step 1 — Simplify the Parallel Part

Assume two resistors of $10\Omega$ are connected in parallel.

Using the parallel formula:

$$
R_p=\frac{R\cdot R}{R+R}
$$

Substitute the values:

$$
R_p=\frac{10\cdot10}{10+10}
$$

$$
R_p=\frac{100}{20}
$$

$$
R_p=5\Omega
$$

So the equivalent resistance of the parallel branch is:

$$
R_p=5\Omega
$$

---

## Step 2 — Add the Series Resistor

Now this equivalent resistance is connected in series with another resistor of $10\Omega$.

For series connection:

$$
R_{eq}=R_s+R_p
$$

Substitute the values:

$$
R_{eq}=10+5
$$

$$
R_{eq}=15\Omega
$$

---

# Final Answer

The equivalent resistance of the circuit is:

$$
\boxed{R_{eq}=15\Omega}
$$