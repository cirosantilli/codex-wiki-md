<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The integral identity requires compactness of $M$, compact support of $X$, or suitable conditions eliminating flux at infinity.** The printed question does not state such a hypothesis. We prove the [Riemannian divergence theorem](../../../../../../riemannian-divergence-theorem.md) for a [compact manifold](../../../../../../compact-manifold.md), and more generally for a [compactly supported](../../../../../../compact-support.md) smooth [vector field](../../../../../../vector-field.md) on an oriented [Riemannian manifold](../../../../../../riemannian-manifold.md) with boundary.

Write $j:\partial M\hookrightarrow M$ for the inclusion. Give $\partial M$ the [outward-normal-first boundary orientation](../../../../../../outward-normal-first-boundary-orientation.md), and let $N$ be the outward unit [normal vector](../../../../../../normal-vector.md). The [Riemannian volume form](../../../../../../riemannian-volume-form.md) of the induced [Riemannian metric](../../../../../../riemannian-metric.md) is

$$
\omega_{\widetilde g}=j^*(\iota_N\omega_g).
$$

Indeed, if $(e_1,\ldots,e_{n-1})$ is a positively oriented [orthonormal basis](../../../../../../orthonormal-basis.md) tangent to the boundary, $(N,e_1,\ldots,e_{n-1})$ is a positively oriented [orthonormal basis](../../../../../../orthonormal-basis.md) in $M$. Both sides therefore evaluate to one on the boundary basis.

At a boundary point decompose $X=g(X,N)N+X^\top$, where $X^\top$ is tangent to $\partial M$. Evaluating on $n-1$ tangent vectors, the term with $X^\top$ vanishes: all $n$ arguments of the alternating [volume form](../../../../../../volume-form.md) then lie in the $(n-1)$-dimensional boundary [tangent space](../../../../../../tangent-space.md). Thus the [interior product of a differential form](../../../../../../interior-product.md) satisfies

$$
j^*(\iota_X\omega_g)=g(X,N)\,\omega_{\widetilde g}.
$$

The general [Stokes theorem](../../../../../../stokes-theorem.md) for an oriented [manifold with boundary](../../../../../../manifold-with-boundary.md) states $\int_M d\eta=\int_{\partial M}j^*\eta$ for any smooth [differential form](../../../../../../differential-form-split.md) $\eta$ of degree $n-1$ with [compact support](../../../../../../compact-support.md); compactness of $M$ makes the support condition automatic. Applying it to $\eta=\iota_X\omega_g$ and using the defining equation for the [divergence of a Riemannian vector field](../../../../../../divergence-of-a-riemannian-vector-field.md) proves

$$
\boxed{\int_M (\operatorname{div}X)\,\omega_g
=\int_{\partial M}g(X,N)\,\omega_{\widetilde g}.}
$$

For a concrete failure without the extra hypothesis, take $M=[0,\infty)$ with [Riemannian metric](../../../../../../riemannian-metric.md) $dx^2$ and $X=(\arctan x)\partial_x$. The [divergence of a Riemannian vector field](../../../../../../divergence-of-a-riemannian-vector-field.md) is $\operatorname{div}X=(1+x^2)^{-1}$, so

$$
\int_M\operatorname{div}X\,dx=\frac\pi2,
\qquad \int_{\partial M}g(X,N)\,\omega_{\widetilde g}=0,
$$

because $X$ vanishes at the only boundary point. Both integrals are finite. The missing $\pi/2$ is the limiting flux at infinity, so mere integrability of the divergence cannot repair the unrestricted assertion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
