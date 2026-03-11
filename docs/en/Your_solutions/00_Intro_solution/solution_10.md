# Infinite Series: Final Position of the Ant

## Useful Definitions and Formulas

### 1. Coordinate Representation of Motion

In two-dimensional motion, the position of an object can be represented by coordinates

$$
(x,y)
$$

where

- $x$ represents horizontal displacement
- $y$ represents vertical displacement

Movements affect coordinates as follows:

- East → increases $x$
- West → decreases $x$
- North → increases $y$
- South → decreases $y$

---

### 2. Infinite Series

An **infinite series** is the sum of infinitely many terms.

It is written as

$$
\sum_{n=1}^{\infty}a_n
$$

If the series approaches a finite value, it is called a **convergent series**.

---

### 3. Alternating Harmonic-Type Series

The movements in this problem form **alternating series** in both the $x$ and $y$ directions.

For example, a common alternating series is

$$
1-\frac13+\frac15-\frac17+\dots
$$

which is known to converge to

$$
\frac{\pi}{4}
$$

Similarly,

$$
\frac12-\frac14+\frac16-\frac18+\dots
$$

converges to

$$
\frac12\ln2
$$

These results allow us to determine the ant's final position.

---

# Step-by-Step Solution

The ant starts at the origin:

$$
(0,0)
$$

It moves according to the pattern:

- $1$ m east
- $\frac12$ m north
- $\frac13$ m west
- $\frac14$ m south
- $\frac15$ m east
- $\frac16$ m north

and the pattern continues indefinitely.

---

# Step 1: Analyze Horizontal Motion

Horizontal movements occur on **odd-numbered steps**.

The pattern is:

East, West, East, West, ...

So the horizontal displacement becomes

$$
x=1-\frac13+\frac15-\frac17+\frac19-\dots
$$

This is a known alternating series.

Its sum is

$$
\frac{\pi}{4}
$$

Thus the total horizontal displacement is

$$
x=\frac{\pi}{4}
$$

---

# Step 2: Analyze Vertical Motion

Vertical movements occur on **even-numbered steps**.

The pattern is:

North, South, North, South, ...

So the vertical displacement becomes

$$
y=\frac12-\frac14+\frac16-\frac18+\frac1{10}-\dots
$$

Factor out $\frac12$:

$$
y=\frac12\left(1-\frac12+\frac13-\frac14+\dots\right)
$$

The series inside the parentheses is known to equal

$$
\ln2
$$

Therefore

$$
y=\frac12\ln2
$$

---

# Step 3: Determine the Final Position

The final coordinates of the ant are

$$
x=\frac{\pi}{4}
$$

$$
y=\frac12\ln2
$$

---

# Final Result

The ant's final position is

$$
\left(\frac{\pi}{4},\frac12\ln2\right)
$$

which is approximately

$$
(0.785,\;0.347)
$$