<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T$ be the $M\times M$ [tridiagonal matrix](../../../../../../tridiagonal-matrix.md) with diagonal two and adjacent entries minus one, incorporating zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md). The actual PDF scheme is

$$
U^{n+1}=G_\mu U^n,\qquad G_\mu=(I+\mu T)^{-1}.
$$

An [orthonormal basis](../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../eigenvector.md) of $T$ has components $\sqrt{2/(M+1)}\sin(jm\pi/(M+1))$, and substitution gives

$$
\lambda_j=2-2\cos\frac{j\pi}{M+1}
=4\sin^2\frac{j\pi}{2(M+1)}>0,\qquad 1\leq j\leq M.
$$

They form an [orthonormal basis](../../../../../../orthonormal-basis.md) by the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md). Hence $I+\mu T$ is invertible for every $\mu>0$, and the amplification [eigenvalues](../../../../../../eigenvalue.md) are $g_j=(1+\mu\lambda_j)^{-1}\in(0,1)$. For the [discrete L2 norm](../../../../../../discrete-l2-norm.md) $\|U\|_h^2=h\sum_m|U_m|^2$,

$$
\boxed{\|G_\mu^n U\|_h\leq\|U\|_h\quad\text{for all }n\geq0,\ \mu>0.}
$$

This bound has constant one independent of time step and mesh, which is the required [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md). Therefore **every positive [Courant number](../../../../../../courant-number.md) is stable**. If a forcing or local-defect sequence is added, the discrete [variation-of-constants formula](../../../../../../variation-of-constants-formula.md) gives a bound by the initial [norm](../../../../../../norm.md) plus the sum of those perturbation [norms](../../../../../../norm.md); this also justifies the [global error](../../../../../../global-discretization-error.md) conclusion in part (a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
