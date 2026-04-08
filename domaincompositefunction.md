# Domain of a Composite Function

This problem requires identifying the set of all possible input values ($x$) for which the function is defined and yields a real number.

---

## 📝 The Question
Find the domain of the following function:
$$f(x) = \frac{\sqrt{4 - x^2}}{\ln(x - 1)}$$

---

## 🛠 Analysis of Constraints
To find the domain, we must satisfy three specific mathematical conditions simultaneously. If any one of these is violated, the function becomes undefined.

### 1. The Even Root Constraint (Numerator)
The expression inside the square root, $4 - x^2$, must be non-negative because the square root of a negative number is not a real number.
$$4 - x^2 \geq 0$$
$$x^2 \leq 4$$
$$-2 \leq x \leq 2$$
**Interval:** $[-2, 2]$

### 2. The Logarithm Constraint (Denominator)
The argument of the natural logarithm, $(x - 1)$, must be strictly positive.
$$x - 1 > 0$$
$$x > 1$$
**Interval:** $(1, \infty)$

### 3. The Rational Constraint (Non-Zero Denominator)
The entire denominator cannot be equal to zero.
$$\ln(x - 1) \neq 0$$
Since $\ln(1) = 0$, the argument $(x - 1)$ cannot be $1$.
$$x - 1 \neq 1$$
$$x \neq 2$$

---

## 🔢 Final Intersection
To find the final domain, we look for the overlap of all three conditions:

, (1, inf), and x != 2]

1.  **Start with the root:** We are limited to the window between $-2$ and $2$.
2.  **Apply the log:** We must be greater than $1$. This narrows our window to $(1, 2]$.
3.  **Apply the non-zero rule:** We must exclude exactly $2$. This changes the closed bracket at $2$ to an open parenthesis.

**Final Answer:**
The domain of the function is:
$$(1, 2)$$

---

## 💡 Key Takeaway
When dealing with complex fractions, always check the **"Big Three"** of domains:
* **Roots:** Can't have a negative under an even root.
* **Logs:** The argument must be strictly positive.
* **Denominators:** Cannot divide by zero.
