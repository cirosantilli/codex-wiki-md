<h1 id="section-d/d17/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**[Orthogonality](../../../../../../orthogonal-vectors.md) means zero [inner product](../../../../../../inner-product-split.md), not merely that two objects look different.** For complex [vectors](../../../../../../vector.md), $\langle u,v\rangle=\sum_i u_i^*v_i$; for [functions](../../../../../../function-split.md) a common choice is $\langle u,v\rangle=\int w(x)u(x)^*v(x)dx$ with positive weight $w$. An [orthonormal set](../../../../../../orthonormal-set.md) has $\langle u_m,u_n\rangle=\delta_{mn}$.

For an [orthogonal](../../../../../../orthogonal-vectors.md) set, the component of $f$ along $u_n$ has coefficient

$$
\boxed{c_n=\frac{\langle u_n,f\rangle}{\langle u_n,u_n\rangle}.}
$$

A complete [orthonormal set](../../../../../../orthonormal-set.md) gives $f=\sum_nc_nu_n$ in the appropriate [norm](../../../../../../norm.md) and [Parseval's identity](../../../../../../parseval-identity.md) $\|f\|^2=\sum_n|c_n|^2$. Without [completeness](../../../../../../completeness.md) there can be a nonzero residual [orthogonal](../../../../../../orthogonal-vectors.md) to the entire chosen set. [Orthogonal](../../../../../../orthogonal-vectors.md) nonzero [vectors](../../../../../../vector.md) are [linearly independent](../../../../../../linear-independence.md), but independence alone does not imply [orthogonality](../../../../../../orthogonal-vectors.md).

[Fourier coefficients](../../../../../../fourier-coefficient.md) are [projections](../../../../../../projection-linear-algebra.md) because

$$
\int_0^T e^{-2\pi imt/T}e^{2\pi int/T}\,dt=T\delta_{mn}.
$$

Likewise, for a [self-adjoint operator](../../../../../../self-adjoint-operator.md), $Au_n=\lambda_nu_n$ gives $(\lambda_n-\lambda_m)\langle u_m,u_n\rangle=0$, so distinct [eigenvalues](../../../../../../eigenvalue.md) have [orthogonal](../../../../../../orthogonal-vectors.md) [eigenvectors](../../../../../../eigenvector.md). Degeneracy does not itself force a chosen pair to be [orthogonal](../../../../../../orthogonal-vectors.md), but an [orthonormal basis](../../../../../../orthonormal-basis.md) can be selected within each [eigenspace](../../../../../../eigenspace.md). The differential version uses the correct Sturm-Liouville weight and [boundary conditions](../../../../../../boundary-condition.md).

For mechanical [normal modes](../../../../../../normal-mode.md) with unequal masses the relevant [inner product](../../../../../../inner-product-split.md) is $\langle u,v\rangle_{\mathsf M}=u^\dagger\mathsf Mv$. This makes the modes in D14 [orthogonal](../../../../../../orthogonal-vectors.md) even when an ordinary unweighted dot product does not. Expanding in such coordinates diagonalizes the kinetic and potential [quadratic forms](../../../../../../quadratic-form-split.md), explaining why modal motions evolve independently and their [energies](../../../../../../energy-split.md) add.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [D17](../../d17.md)
3. [Section D](../../../section-d.md)
4. [Paper 2A](../../../../paper-2a-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
