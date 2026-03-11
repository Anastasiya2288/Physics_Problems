# Optimization Problem: Maximum Area Rectangle

## Useful Definitions and Formulas

### 1. Optimization

**Optimization** in calculus means finding the **maximum or minimum value** of a function.

In many geometry problems, we first express the quantity to optimize (such as area or volume) as a **function**, and then find where that function reaches its maximum or minimum.

---

### 2. Area of a Rectangle

The area of a rectangle is

$$
A=width\cdot height
$$

If the width and height depend on a variable $x$, then the area becomes a function

$$
A(x)
$$

which we can analyze to find its maximum value.

---

### 3. Derivatives and Critical Points

To find a maximum or minimum of a function:

1. Compute the derivative

$$
A'(x)
$$

2. Find the **critical points** by solving

$$
A'(x)=0
$$

3. Use these points to determine where the function reaches its **maximum value**.

---

# Step-by-Step Solution

We are given the curve

$$
y=3-x^2
$$

and a rectangle located **under the curve in the first quadrant**.

This means:

- The rectangle's top-right corner lies on the curve.
- The rectangle touches the axes.

---

# Step 1: Express the Dimensions of the Rectangle

Let the top-right corner of the rectangle be

$$
(x,y)
$$

Since the point lies on the curve,

$$
y=3-x^2
$$

Thus:

Width of the rectangle:

$$
x
$$

Height of the rectangle:

$$
3-x^2
$$

---

# Step 2: Express the Area Function

The area of the rectangle is

$$
A=width\cdot height
$$

Substitute the expressions:

$$
A(x)=x(3-x^2)
$$

Expand the expression:

$$
A(x)=3x-x^3
$$

---

# Step 3: Compute the Derivative

Differentiate the area function:

$$
A'(x)=\frac{d}{dx}(3x-x^3)
$$

$$
A'(x)=3-3x^2
$$

---

# Step 4: Find Critical Points

Set the derivative equal to zero:

$$
3-3x^2=0
$$

Divide both sides by $3$:

$$
1-x^2=0
$$

$$
x^2=1
$$

Since we are in the **first quadrant**, we take

$$
x=1
$$

---

# Step 5: Find the Height

Substitute $x=1$ into the curve equation:

$$
y=3-x^2
$$

$$
y=3-1^2
$$

$$
y=3-1
$$

$$
y=2
$$

---

# Step 6: Determine the Maximum Area

The rectangle dimensions are

Width:

$$
1
$$

Height:

$$
2
$$

Area:

$$
A=1\cdot2=2
$$

---

# Final Result

The rectangle with maximum area has dimensions

Width:

$$
1
$$

Height:

$$
2
$$

Maximum area:

$$
2
$$