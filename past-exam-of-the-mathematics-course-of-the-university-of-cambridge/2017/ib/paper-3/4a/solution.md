<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Let $Y(s)$ be the [Laplace transform](../../../../../laplace-transform.md) of $y$. The initial values give $\mathcal L(y')=sY$ and $\mathcal L(y'')=s^2Y-1$, while $\mathcal L(te^{-3t})=(s+3)^{-2}$. Therefore, for $\operatorname{Re}s$ sufficiently large,

$$
(s^2-4s+3)Y(s)-1=\frac1{(s+3)^2},\qquad
Y(s)=\frac{1+(s+3)^{-2}}{(s-1)(s-3)}.
$$

The [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is

$$
Y(s)=\frac{37}{72(s-3)}-\frac{17}{32(s-1)}+\frac5{288(s+3)}+\frac1{24(s+3)^2}.
$$

Inverting the elementary [Laplace transforms](../../../../../laplace-transform.md) gives

$$
\boxed{y(t)=\frac{37}{72}e^{3t}-\frac{17}{32}e^t+\left(\frac5{288}+\frac t{24}\right)e^{-3t},\qquad t\ge0.}
$$

These coefficients give $y(0)=0$ and $y'(0)=1$; the transformed equation, or direct differentiation, verifies the forcing. Uniqueness follows from uniqueness for the corresponding linear initial-value [ordinary differential equation](../../../../../ordinary-differential-equation.md).

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
