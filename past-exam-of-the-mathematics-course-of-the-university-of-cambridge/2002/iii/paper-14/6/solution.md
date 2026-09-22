<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

On an oriented Riemannian $n$-manifold, the [metric volume form](../../../../../metric-volume-form.md) is the unique top form taking value one on every positively oriented orthonormal tangent basis. In a positive coordinate chart it is

$$
\boxed{\operatorname{vol}_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n}.
$$

For another positive coordinate chart $y$, write $A=\partial x/\partial y$. Then $g_y=A^{\mathsf T}g_xA$, so $\sqrt{\det g_y}=\det A\sqrt{\det g_x}$, since $\det A>0$. The wedge of coordinate differentials acquires the same [determinant](../../../../../determinant.md) factor. The two local expressions agree, proving coordinate independence and smooth global existence. Positivity of the chosen charts is what fixes the sign of the [volume form](../../../../../volume-form.md).

The metric induces the [inner product on exterior powers of a cotangent space](../../../../../inner-product-on-exterior-powers-of-a-cotangent-space.md). Define the [Hodge star operator](../../../../../hodge-star-operator.md) $*:\Lambda^pT^*M\to\Lambda^{n-p}T^*M$ by

$$
\boxed{\alpha\wedge*\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g}
$$

for forms of the same degree, and apply it fiberwise to smooth forms. In an oriented orthonormal coframe, if $I$ is an increasing $p$-index and $I^c$ its ordered complement, $*e^I=\epsilon(I,I^c)e^{I^c}$. Exchanging the two blocks has sign $(-1)^{p(n-p)}$, so

$$
\boxed{*^2|_{\Omega^p}=(-1)^{p(n-p)}I}.
$$

Use the real $L^2$ [inner product](../../../../../inner-product.md) $(\alpha,\beta)=\int_M\alpha\wedge*\beta$. For a $p$-form $\alpha$ and a $(p+1)$-form $\beta$, the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) and the given boundaryless Stokes identity give

$$
0=\int_M d(\alpha\wedge*\beta)
=\int_M d\alpha\wedge*\beta+(-1)^p\int_M\alpha\wedge d*\beta.
$$

The [codifferential](../../../../../codifferential.md) acting on $\beta$ has sign $(-1)^{n(p+2)+1}$. Applying the star once more and using its square on the $(n-p)$-form $d*\beta$ gives

$$
*\delta\beta=(-1)^{n(p+2)+1+p(n-p)}d*\beta=(-1)^{p+1}d*\beta.
$$

The exponent reduction uses parity, since $p^2\equiv p\pmod2$. Combining the two displayed identities proves $(d\alpha,\beta)=(\alpha,\delta\beta)$. Symmetry of the real [inner product](../../../../../inner-product.md) supplies precisely

$$
\boxed{\int_M\beta\wedge*d\alpha=\int_M\delta\beta\wedge*\alpha}.
$$

Thus [Hodge integration by parts in arbitrary degree](../../../../../hodge-integration-by-parts-in-arbitrary-degree.md) identifies $\delta$ as the formal adjoint of $d$. The displayed bilinear identity extends to complex [differential forms](../../../../../differential-form-split.md) by complex linearity. For positive norm identities on complex forms, use the Hermitian [inner product](../../../../../inner-product.md) with conjugation instead.

With the nonnegative convention, the [Hodge Laplacian](../../../../../hodge-laplacian.md) is

$$
\boxed{\Delta=d\delta+\delta d}.
$$

It is the form-valued extension of the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md), whose action on functions is $-\operatorname{div}\operatorname{grad}$. A [harmonic differential form](../../../../../harmonic-differential-form.md) is a smooth form in $\ker\Delta$. The adjoint identity gives

$$
(\Delta\alpha,\alpha)=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2.
$$

If $\Delta\alpha=0$, both norms vanish, and smoothness implies

$$
\boxed{d\alpha=0,\qquad\delta\alpha=0}.
$$

The closed compact hypotheses are essential for the absence of boundary terms and this global energy conclusion.

The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) states that on a closed oriented [Riemannian manifold](../../../../../riemannian-manifold.md)

$$
\boxed{\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M)}
$$

is an $L^2$-orthogonal direct sum, with finite-dimensional harmonic space $\mathcal H^p$. Every smooth form has unique harmonic, exact and coexact components, although primitives of the latter two need not be unique. Equivalently every [de Rham cohomology](../../../../../de-rham-cohomology.md) class has a unique harmonic representative. An exact harmonic form belongs to both the harmonic and exact summands; their orthogonality makes its squared norm zero. Therefore $\boxed{\alpha\text{ exact and harmonic}\Longrightarrow\alpha=0}$. The same conclusion follows directly from $\alpha=d\eta$ and $\|\alpha\|^2=(\delta\alpha,\eta)=0$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
