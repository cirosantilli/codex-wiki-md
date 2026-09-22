<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For real [smooth functions](../../../../../../smooth-function.md) of [compact support](../../../../../../compact-support.md) in a planar [domain](../../../../../../domain-mathematical-analysis.md) $D$, use the [Dirichlet inner product](../../../../../../dirichlet-inner-product.md)

$$
\boxed{(u,v)_{\nabla,D}=\frac1{2\pi}\int_D\nabla u\cdot\nabla v\,dA.}
$$

Changing the positive normalization factor does not change [orthogonality](../../../../../../orthogonal-vectors.md). For complex functions, insert [complex conjugation](../../../../../../complex-conjugation.md) in the second factor to obtain the corresponding [Hermitian form](../../../../../../hermitian-form.md).

Let $f:D\to\widetilde D$ be a [conformal bijection](../../../../../../biholomorphism.md), and let $\widetilde u,\widetilde v$ be [smooth functions](../../../../../../smooth-function.md) of [compact support](../../../../../../compact-support.md) on $\widetilde D$. Its real [Jacobian matrix](../../../../../../jacobian-matrix.md) is $Df=|f'|R$, where $R$ is a rotation. By the [chain rule](../../../../../../chain-rule.md),

$$
\nabla(\widetilde u\circ f)\cdot\nabla(\widetilde v\circ f)=|f'|^2(\nabla\widetilde u\cdot\nabla\widetilde v)\circ f.
$$

The [change of variables formula](../../../../../../change-of-variables-formula.md) has [Jacobian determinant](../../../../../../jacobian-determinant.md) $|f'|^2$, so this factor cancels:

$$
\boxed{(\widetilde u\circ f,\widetilde v\circ f)_{\nabla,D}=(\widetilde u,\widetilde v)_{\nabla,\widetilde D}.}
$$

This proves [conformal invariance of the planar Dirichlet inner product](../../../../../../conformal-invariance-of-the-planar-dirichlet-inner-product.md). By completion it is also an [isometry](../../../../../../isometry.md) between the corresponding [Dirichlet energy spaces](../../../../../../dirichlet-energy-space.md). It asserts invariance of the energy form, not of the inhomogeneous [Sobolev norm](../../../../../../sobolev-norm.md), whose $L^2$ term has a different transformation rule.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
