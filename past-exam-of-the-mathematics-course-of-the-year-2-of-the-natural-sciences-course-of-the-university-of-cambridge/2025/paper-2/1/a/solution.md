<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Multiplication by $x^2$ gives the [Sturm-Liouville form](../../../../../sturm-liouville-form.md)

$$
-(x^2u')'=\lambda x^2u,
$$

so the weight is $w(x)=x^2$. Use the weighted [inner product](../../../../../inner-product-split.md) $\langle f,g\rangle_w=\int_0^{\pi/2}x^2\overline f g\,dx$ and the [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) $L=-x^{-2}(x^2d/dx)'$. [Integration by parts](../../../../../integration-by-parts.md) gives its boundary form:

$$
\langle f,Lg\rangle_w-\langle Lf,g\rangle_w
=\left[x^2(\overline {f'}g-\overline f g')\right]_0^{\pi/2}=0.
$$

The upper endpoint term vanishes by the [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), and the lower one vanishes for the regular solutions. More precisely, the [radial Dirichlet spectrum in three dimensions](../../../../../radial-dirichlet-spectrum-in-three-dimensions.md) identifies $L$ under the [unitary transformation](../../../../../unitary-operator.md) $v=xu$ with $-v''$ on $(0,\pi/2)$ with zero endpoint values; this specifies the [self-adjoint](../../../../../self-adjoint-operator.md) realization at the singular endpoint as well as proving the formal identity.

For [eigenfunctions](../../../../../eigenfunction.md) $u_a,u_b$ with different [eigenvalues](../../../../../eigenvalue.md), the same identity gives $(\lambda_b-\lambda_a)\langle u_a,u_b\rangle_w=0$. Taking real [eigenfunctions](../../../../../eigenfunction.md) proves the required [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
