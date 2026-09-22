<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Invert the equation and regard $x$ as a function of $y$:

$$
\frac{dx}{dy}-x=e^{2y}.
$$

This is a [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md). Multiplication by the [integrating factor](../../../../../integrating-factor.md) $e^{-y}$ gives

$$
\frac d{dy}(xe^{-y})=e^y,
$$

so $x=e^{2y}+Ce^y$. The initial condition $x=1$ at $y=0$ gives $C=0$. Hence $x=e^{2y}$ and

$$
\boxed{y(x)=\frac12\log x},
\qquad x>0.
$$

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
