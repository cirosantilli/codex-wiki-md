<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On its specified domain of admissible functions, a [self-adjoint operator](../../../../../self-adjoint-operator.md) equals its adjoint, including the adjoint domain. Its integration identity on the interval is

$$
\boxed{\langle u,Lv\rangle=\langle Lu,v\rangle,\qquad\langle u,v\rangle=\int_a^b u^*(x)v(x)\,dx.}
$$

For a differential operator, the boundary conditions must make the boundary form from [integration by parts](../../../../../integration-by-parts.md) vanish. Formal symmetry of the differential expression alone does not specify a self-adjoint boundary-value problem.

Apply this identity to two [eigenfunctions](../../../../../eigenfunction.md). Since the weight is real,

$$
\lambda_n\int_a^b wy_m^*y_n\,dx=\int_a^b y_m^*Ly_n\,dx=\int_a^b(Ly_m)^*y_n\,dx=\lambda_m^*\int_a^b wy_m^*y_n\,dx.
$$

First take $m=n$: positivity of $\int_a^b w|y_n|^2dx$ shows $\lambda_n=\lambda_n^*$, so the [eigenvalues](../../../../../eigenvalue.md) are real. For distinct eigenvalues, subtraction therefore gives

$$
\boxed{\int_a^b w(x)y_m^*(x)y_n(x)\,dx=0\quad(\lambda_m\ne\lambda_n).}
$$

This is [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) in the [weighted inner product](../../../../../weighted-inner-product.md), rather than necessarily in the unweighted inner product.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
