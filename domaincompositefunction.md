# 微積分：函數定義域 (Domain of a Function)

This problem is a classic example of finding the domain of a composite function, a frequent topic in Taiwan's University Transfer Exams (轉學考).

---

## 📝 Problem Statement
Find the domain of the function:
$$f(x) = \frac{\sqrt{4 - x^2}}{\ln(x - 1)}$$

---

## 🛠 Analysis & Solution

To find the domain $D_f$, we must ensure the function is defined within the set of real numbers $\mathbb{R}$. This requires satisfying the following three constraints simultaneously:

### 1. Radicand Constraint (根號限制)
For an even-indexed root to be defined in $\mathbb{R}$, the radicand must be non-negative:
$$4 - x^2 \geq 0$$
$$(2-x)(2+x) \geq 0$$
$$-2 \leq x \leq 2 \quad \cdots \text{(I)}$$

### 2. Logarithmic Constraint (對數限制)
The argument of the natural logarithm must be strictly positive:
$$x - 1 > 0$$
$$x > 1 \quad \cdots \text{(II)}$$

### 3. Non-zero Denominator Constraint (分母不為零限制)
The denominator of a fraction cannot be zero:
$$\ln(x - 1) \neq 0$$
Since $\ln(1) = 0$, we have:
$$x - 1 \neq 1$$
$$x \neq 2 \quad \cdots \text{(III)}$$

---

## 🔢 Final Intersection (交集)

We determine the domain by finding the intersection of sets (I), (II), and (III):
$$D_f = \{x \in \mathbb{R} \mid -2 \leq x \leq 2\} \cap \{x \in \mathbb{R} \mid x > 1\} \cap \{x \in \mathbb{R} \mid x \neq 2\}$$

1. From (I) and (II): $1 < x \leq 2$.
2. Applying (III) ($x \neq 2$): The upper bound becomes strictly less than 2.



**Final Answer:**
The domain in interval notation is:
$$(1, 2)$$

---

## 💡 Exam Tips for Taiwan Transfer Exams
* **Notation:** In Taiwan exams, you can provide the answer in set notation $\{x \mid 1 < x < 2\}$ or interval notation $(1, 2)$. Both are generally accepted unless specified.
* **Partial Credit:** Always list the three constraints (Radical, Log, Denominator) separately. Even if you make a calculation error at the end, identifying these will usually earn you partial points.
* **Boundary Check:** Pay close attention to whether the endpoints (1 and 2) are included (closed bracket) or excluded (open parenthesis). This is the most common place students lose marks.
