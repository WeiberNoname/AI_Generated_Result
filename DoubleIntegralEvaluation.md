# Double Integral Evaluation

To evaluate the double integral $\iint_R 20x^2e^{-y} dA$ over the rectangular region $R$, we use the given boundaries:
$R = \{(x, y) : 0 \leq x \leq 3, 0 \leq y \leq 2\}$.

## 1. Set up the Iterated Integral
Since the limits of integration are constants and the integrand is a product of functions of $x$ and $y$, we can separate the integral:

$$\int_{0}^{3} \int_{0}^{2} 20x^2 e^{-y} \, dy \, dx = 20 \left( \int_{0}^{3} x^2 \, dx \right) \left( \int_{0}^{2} e^{-y} \, dy \right)$$

## 2. Evaluate the Integrals

### Part A: The $x$-component
Using the power rule:
$$\int_{0}^{3} x^2 \, dx = \left[ \frac{x^3}{3} \right]_{0}^{3} = \frac{27}{3} - 0 = 9$$

### Part B: The $y$-component
Using the exponential rule $\int e^{au} du = \frac{1{a}}e^{au}$:
$$\int_{0}^{2} e^{-y} \, dy = \left[ -e^{-y} \right]_{0}^{2} = (-e^{-2}) - (-e^{0})$$
$$\int_{0}^{2} e^{-y} \, dy = 1 - e^{-2}$$

## 3. Final Calculation
Multiply the results together with the constant factor:

$$\text{Value} = 20 \cdot 9 \cdot (1 - e^{-2})$$
$$\text{Value} = 180(1 - e^{-2})$$

---
**Numerical Approximation:** $180(1 - e^{-2}) \approx 155.64$

# Evaluating the Double Integral

$$\iint_R 20x^2e^{-y}\,dA, \quad R = \{(x,y): 0 \leq x \leq 3,\ 0 \leq y \leq 2\}$$

Since the region $R$ is a rectangle, we can separate the integral into a product of two single integrals.

---

## Step 1: Set Up as Iterated Integral

$$\int_0^2 \int_0^3 20x^2e^{-y}\,dx\,dy$$

Since $20x^2e^{-y} = 20x^2 \cdot e^{-y}$, we can **factor and separate**:

$$= 20\left(\int_0^3 x^2\,dx\right)\left(\int_0^2 e^{-y}\,dy\right)$$

---

## Step 2: Evaluate the x-integral

$$\int_0^3 x^2\,dx = \left[\frac{x^3}{3}\right]_0^3 = \frac{27}{3} - 0 = 9$$

---

## Step 3: Evaluate the y-integral

$$\int_0^2 e^{-y}\,dy = \left[-e^{-y}\right]_0^2 = -e^{-2} - (-e^{0}) = 1 - e^{-2}$$

---

## Step 4: Multiply Everything Together

$$20 \cdot 9 \cdot (1 - e^{-2})$$

$$= 180(1 - e^{-2})$$

---

## Final Answer

$$\boxed{180\left(1 - e^{-2}\right) \approx 155.7}$$
