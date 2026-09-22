<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $H=-\partial_x^2+V(x)$. The real potential and periodic boundary conditions make $H$ a [self-adjoint operator](../../../../../../self-adjoint-operator.md). Since $u_t=-iHu$,

$$
\frac d{dt}\int_{-1}^1|u|^2dx
=2\operatorname{Re}\int_{-1}^1\overline u,u_tdx
=2\operatorname{Re}\left(-i\int_{-1}^1\overline u,Hu\,dx\right)=0,
$$

because the expectation of a self-adjoint operator is real. Equivalently, integrating the kinetic term by parts leaves $\int|u_x|^2dx$ and the periodic boundary term cancels. Thus the continuous [Schrödinger equation](../../../../../../schrodinger-equation.md) preserves its $L^2$ norm.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
