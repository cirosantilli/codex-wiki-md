<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [integrating factor](../../../../../../integrating-factor.md) explains the second hint and the first-order inner calculation. For

$$
Y''+2zY'=2a_1z+a_2+a_3\operatorname{erf}z,
$$

multiplication by $e^{z^2}$ gives $(e^{z^2}Y')'=e^{z^2}(2a_1z+a_2+a_3\operatorname{erf}z)$. The term $a_1z$ already produces $2a_1z$, and integrating the remaining terms twice gives $a_2E_0+a_3E_1$, in terms of the [Gaussian drift primitives](../../../../../../gaussian-drift-primitives.md). The [homogeneous solutions](../../../../../../homogeneous-solution.md) are a constant and the [error function](../../../../../../error-function.md). Hence

$$
\boxed{Y=a_1z+a_2E_0(z)+a_3E_1(z)+K_0+K_1\operatorname{erf}z.}
$$

For the piecewise forcing in the inner problem, $F$ replaces $a_1z$ and provides the continuously matched particular solution for $2zH(-z)$. The coefficients $2c$ and $2d$ then account for the $2Y_0$ forcing.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
