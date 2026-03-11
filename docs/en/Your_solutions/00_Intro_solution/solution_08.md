# Definite Integrals: Area Under the Curve

## Useful Definitions and Formulas

### 1. Definite Integral

A **definite integral** represents the **area under a curve** of a function between two points on the $x$-axis.

The definite integral of a function $f(x)$ from $a$ to $b$ is written as

$$
\int_a^b f(x)\,dx
$$

This represents the **area between the graph of the function and the $x$-axis** from $x=a$ to $x=b$.

---

### 2. Fundamental Theorem of Calculus

The **Fundamental Theorem of Calculus** states that if $F(x)$ is an antiderivative of $f(x)$, then

$$
\int_a^b f(x)\,dx = F(b)-F(a)
$$

where $F'(x)=f(x)$.

---

### 3. Integral of the Sine Function

A key integral used in this problem is

$$
\int \sin x\,dx = -\cos x + C
$$

Therefore the antiderivative of $\sin x$ is

$$
F(x)=-\cos x
$$

---

# Step-by-Step Solution

We are asked to compute the area under the curve

$$
f(x)=\sin x
$$

from

$$
x=0
$$

to

$$
x=\pi
$$

Thus the definite integral is

$$
\int_0^\pi \sin x\,dx
$$

---

# Step 1: Find the Antiderivative

The antiderivative of $\sin x$ is

$$
-\cos x
$$

So

$$
\int \sin x\,dx=-\cos x
$$

---

# Step 2: Apply the Fundamental Theorem of Calculus

Using

$$
\int_a^b f(x)\,dx=F(b)-F(a)
$$

we obtain

$$
\int_0^\pi \sin x\,dx = -\cos x\Big|_0^\pi
$$

---

# Step 3: Evaluate at the Limits

Substitute the limits:

$$
-\cos\pi - (-\cos0)
$$

---

# Step 4: Use Trigonometric Values

Known cosine values:

$$
\cos\pi=-1
$$

$$
\cos0=1
$$

Substitute them:

$$
-\cos\pi = -(-1)
$$

$$
=1
$$

and

$$
-\cos0 = -1
$$

Now compute the difference:

$$
1-(-1)
$$

$$
=2
$$

---

# Final Result

The area under the curve of $f(x)=\sin x$ from $0$ to $\pi$ is

$$
2
$$