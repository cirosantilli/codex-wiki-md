<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

[Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot E=\rho/\varepsilon_0,\quad \nabla\cdot B=0,
\quad\nabla\times E=-\partial_tB,
\quad\nabla\times B=\mu_0J+\mu_0\varepsilon_0\partial_tE.
$$

Taking the divergence of the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) and using [Gauss's law](../../../../../gauss-s-law.md) gives

$$
\partial_t\rho+\nabla\cdot J=0.
$$

Therefore

$$
\dot Q=-\int_{\partial D}J\cdot n\,dS=0
$$

because $J$ vanishes on the boundary. Componentwise integration by parts also gives

$$
\frac d{dt}\int_Dx\rho\,d^3x=-\int_Dx\nabla\cdot J\,d^3x=\int_DJ\,d^3x,
$$

with the boundary term again zero.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
