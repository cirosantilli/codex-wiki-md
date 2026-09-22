<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the two-dimensional dependence as independence of $z$, allowing the velocity to have a vertical component $U=u_z(x,y)$. Write $u_h=(u_x,u_y)$ and $B_h=(A_y,-A_x)$. The [resistive induction equation](../../../../../../resistive-induction-equation.md), with a gauge fixing the potential's zero mean, gives

$$
A_t+u_h\cdot\nabla A=\eta\nabla^2A,\qquad
B_t+u_h\cdot\nabla B=B_h\cdot\nabla U+\eta\nabla^2B.
$$

The first is a homogeneous [advection-diffusion equation](../../../../../../advection-diffusion-equation.md). Multiply it by $A$, average over the periodic box and use [integration by parts](../../../../../../integration-by-parts.md). Advection contributes zero because $\nabla\cdot u_h=0$; there are no surface terms. Thus

$$
\frac12\frac{d}{dt}\langle A^2\rangle=-\eta\langle|\nabla A|^2\rangle
\leq-\eta k^2\langle A^2\rangle.
$$

Multiplying by $e^{2\eta k^2t}$ makes its derivative nonpositive. With the initial norm convention $\langle A^2(0)\rangle=A_0^2$, this proves

$$
\boxed{\langle A^2(t)\rangle\leq A_0^2e^{-2\eta k^2t}.}
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) uses the zero-mean assumption; a spatially constant flux potential would otherwise have no gradient. Zero mean remains preserved by this incompressible periodic equation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
