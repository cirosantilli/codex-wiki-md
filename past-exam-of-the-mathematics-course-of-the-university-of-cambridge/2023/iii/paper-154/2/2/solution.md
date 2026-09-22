<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Differentiate the energy and use the [chain rule](../../../../../../chain-rule.md):

$$
\frac{dE}{dt}
=\int_{\mathbb R^3}
\left(u_tu_{tt}+\nabla u\cdot\nabla u_t+|u|^{p-1}uu_t\right)dx.
$$

After [integration by parts](../../../../../../integration-by-parts.md), the middle term is $-\int(\Delta u)u_t$. Therefore

$$
\frac{dE}{dt}
=\int u_t\left(u_{tt}-\Delta u+u|u|^{p-1}\right)dx=0
$$

by the [defocusing semilinear wave equation](../../../../../../defocusing-semilinear-wave-equation.md). Thus the total energy is conserved.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
