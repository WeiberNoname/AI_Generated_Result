# 微積分：泰勒級數展開 (Taylor Series Expansion)

In transfer exams, finding a Taylor series for rational functions is best approached using geometric series manipulation rather than calculating high-order derivatives.

---

## 📝 Problem Statement
Find the Taylor series (Maclaurin series) of the function:
$$f(x) = \frac{x}{3 + 2x}$$

---

## 🛠 Analysis & Solution

### 1. Recall the Geometric Series (回顧幾何級數)
The standard power series expansion is:
$$\frac{1}{1 - u} = \sum_{n=0}^{\infty} u^n = 1 + u + u^2 + u^3 + \dots \quad \text{for } |u| < 1$$

### 2. Algebraic Manipulation (代數變形)
We need to rewrite $f(x)$ to match the form $\frac{1}{1 - u}$. 

First, factor out $3$ from the denominator:
$$f(x) = \frac{x}{3(1 + \frac{2x}{3})}$$
$$f(x) = \frac{x}{3} \cdot \frac{1}{1 - (-\frac{2x}{3})}$$

### 3. Expansion
Now, substitute $u = -\frac{2x}{3}$ into the geometric series formula:
$$\frac{1}{1 - (-\frac{2x}{3})} = \sum_{n=0}^{\infty} \left( -\frac{2x}{3} \right)^n$$
$$\frac{1}{1 - (-\frac{2x}{3})} = \sum_{n=0}^{\infty} (-1)^n \frac{2^n}{3^n} x^n$$

### 4. Incorporate the Exterior Term
Multiply the entire series by the factor $\frac{x}{3}$ we set aside:
$$f(x) = \frac{x}{3} \sum_{n=0}^{\infty} (-1)^n \frac{2^n}{3^n} x^n$$
$$f(x) = \sum_{n=0}^{\infty} (-1)^n \frac{2^n}{3^{n+1}} x^{n+1}$$

---

## 🔢 Final Result
The Taylor series for $f(x)$ centered at $x=0$ is:
$$f(x) = \sum_{n=0}^{\infty} \frac{(-1)^n 2^n}{3^{n+1}} x^{n+1}$$
*Expanded form:* $\frac{1}{3}x - \frac{2}{9}x^2 + \frac{4}{27}x^3 - \frac{8}{81}x^4 + \dots$

### Radius of Convergence (收斂半徑)
The expansion is valid when $|u| < 1$:
$$\left| -\frac{2x}{3} \right| < 1 \implies |x| < \frac{3}{2}$$
Thus, the radius of convergence is $R = \frac{3}{2}$.

---

## 💡 Exam Tips for Taiwan Transfer Exams
* **Method Choice:** Do not use the definition $f^{(n)}(0)/n!$ for rational functions. It takes too long and is prone to calculation errors. Geometric series substitution is the "gold standard" for these problems.
* **The $x$ term:** Don't forget to shift the index or the power of $x$ if there is an $x$ in the numerator. Notice how the final power is $x^{n+1}$.
* **Interval of Convergence:** Many exams in Taiwan (like NTU or UST) will award extra points (or avoid losing them) if you explicitly state the radius or interval of convergence, even if the question only asks for the series.
