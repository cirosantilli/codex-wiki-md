<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the standard convention that these compact [smooth manifolds](../../../../../../smooth-manifold.md) have no boundary. The [interior product](../../../../../../interior-product.md) identity for a one-form gives $df\wedge\iota_X\omega_g=df(X)\omega_g=X(f)\omega_g$. For example, in the [coframe](../../../../../../coframe.md) from part (b), only the matching index survives in this wedge product, with the same pair of cancelling signs as in part (c). Thus the graded [Leibniz rule](../../../../../../leibniz-rule.md) and part (c) give

$$
d(f\nu)=df\wedge\nu+f\,d\nu
=\bigl(X(f)+f\operatorname{div}X\bigr)\omega_g.
$$

Integrate and apply the [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md). Since $\partial M=\varnothing$, the integral of $d(f\nu)$ is zero. Rearranging proves [integration by parts for Riemannian divergence](../../../../../../integration-by-parts-for-riemannian-divergence.md):

$$
\boxed{\int_M X(f)\omega_g=-\int_M f\operatorname{div}X\,\omega_g.}
$$

If a boundary were allowed, the exact general formula would instead have the additional term $\int_{\partial M}f\nu$ on the right; [compactness](../../../../../../compact-space.md) alone does not remove that boundary contribution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
