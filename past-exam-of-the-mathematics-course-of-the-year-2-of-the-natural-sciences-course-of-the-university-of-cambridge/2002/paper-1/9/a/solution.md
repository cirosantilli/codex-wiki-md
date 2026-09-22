<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the real [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) $\mathcal Ly=-(py')'+qy$, two integrations by parts give the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md):

$$
\int_0^1(u\mathcal Lv-v\mathcal Lu)\,dx=[p(vu'-uv')]_0^1.
$$

Set $u=y_n,v=\widetilde y$. Both vanish at the endpoints, so the boundary term is zero. Since $\mathcal Ly_n=\lambda_nwy_n$,

$$
\int_0^1y_n\mathcal L\widetilde y\,dx=\int_0^1\widetilde y\mathcal Ly_n\,dx=\lambda_n\int_0^1wy_n\widetilde y\,dx.
$$

Consequently

$$
\boxed{\int_0^1y_nF_n\,dx=\int_0^1y_n(\mathcal L\widetilde y-\lambda_nw\widetilde y)\,dx=0.}
$$

This is [self-adjointness](../../../../../self-adjoint-operator.md) with the homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), and expresses the [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) at the [eigenvalue](../../../../../eigenvalue.md) $\lambda_n$. In this unweighted integral $F_n$ already contains its factor of $w$; adding another weight would be incorrect.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
