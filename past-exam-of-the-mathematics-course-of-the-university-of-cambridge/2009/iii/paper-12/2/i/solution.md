<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $H^1=W^{1,2}$ and $H_0^1=W_0^{1,2}$. The [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) in the [Sobolev space](../../../../../../sobolev-space-split.md) sense means $u-\psi\in H_0^1(\Omega)$; this definition remains meaningful even without regularity assumptions on the boundary. For bounded full coefficients, a [weak solution](../../../../../../weak-solution.md) is a function satisfying

$$
\boxed{u\in H^1(\Omega),\quad u-\psi\in H_0^1(\Omega),\quad B(u,\varphi)=-\int_\Omega f\varphi\quad\text{for every }\varphi\in H_0^1(\Omega),}
$$

where

$$
B(u,\varphi)=\int_\Omega a_{ij}D_ju\,D_i\varphi-\int_\Omega qu\varphi.
$$

The sign follows by [integration by parts](../../../../../../integration-by-parts.md) in $D_i(a_{ij}D_ju)+qu=f$. No classical derivatives of the measurable coefficients are taken. Equivalently one may first test against $C_c^\infty(\Omega)$ and extend by density, provided this [bilinear form](../../../../../../bilinear-form.md) is bounded on $H^1\times H_0^1$. All integrals in this definition must exist: as explained below, the printed quadratic bounds alone do not guarantee this when $A=(a_{ij})$ is nonsymmetric.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
