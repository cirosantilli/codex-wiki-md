<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Use the real [weighted inner product](../../../../weighted-inner-product.md) $\langle u,v\rangle_w=\int_a^bwuv\,dx$ and the energy bilinear form $B(u,v)=\int_a^b(pu'v'+quv)dx$. [Integration by parts](../../../../integration-by-parts.md), the endpoint conditions, and the [Sturm-Liouville problem](../../../../sturm-liouville-problem.md) give

$$
B(y_i,y_j)=\int_a^by_i[-(py_j')'+qy_j]dx=\lambda_j\langle y_i,y_j\rangle_w=\lambda_j\delta_{ij}.
$$

Thus [orthonormality](../../../../orthonormal-set.md) in the stated expansion gives

$$
F[y_{\rm trial}]=A^2\left(\lambda_0+\sum_{i\geq1}c_i^2\lambda_i\right),\qquad G[y_{\rm trial}]=A^2\left(1+\sum_{i\geq1}c_i^2\right),
$$

and hence the [Rayleigh quotient](../../../../rayleigh-quotient.md)

$$
\boxed{\lambda_{\rm trial}=\frac{\lambda_0+\sum_{i\geq1}c_i^2\lambda_i}{1+\sum_{i\geq1}c_i^2}.}
$$

The expansion is understood for nonzero admissible functions with finite norm and energy.

For a general endpoint-preserving variation $y+\varepsilon\eta$, explicitly

$$
\delta F=2\int_a^b[-(py')'+qy]\eta\,dx,\qquad\delta G=2\int_a^bwy\eta\,dx,
$$

so

$$
\delta\Lambda=\frac{\delta F-\Lambda\delta G}{G}=\frac2G\int_a^b[-(py')'+qy-\Lambda wy]\eta\,dx.
$$

The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) shows that stationarity is exactly the [eigenvalue](../../../../eigenvalue.md) equation with $\lambda=\Lambda$. Conversely an [eigenfunction](../../../../eigenfunction.md) has vanishing first variation and quotient equal to its [eigenvalue](../../../../eigenvalue.md). Completeness gives the same weighted-average formula for any nonzero admissible expansion, even one with zero ground-state coefficient. Since every $\lambda_i\geq\lambda_0$,

$$
\boxed{\Lambda[y]\geq\lambda_0.}
$$

This is the [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md).

For the interval problem, the normalized [Dirichlet eigenfunctions](../../../../dirichlet-eigenfunction.md) and their [eigenvalues](../../../../eigenvalue.md), with the paper's zero-based indexing, are

$$
y_i(x)=\sqrt2\sin[(i+1)\pi x],\qquad\lambda_i=(i+1)^2\pi^2.
$$

For $u=x(1-x)$, direct integration gives $F=\int_0^1(1-2x)^2dx=1/3$ and $G=\int_0^1x^2(1-x)^2dx=1/30$. Therefore

$$
\boxed{\lambda_{\rm trial}=10>\lambda_0=\pi^2.}
$$

The [sine expansion and Rayleigh quotient of a parabolic Dirichlet trial](../../../../sine-expansion-and-rayleigh-quotient-of-a-parabolic-dirichlet-trial.md) follow from the coefficient integral

$$
\int_0^1x(1-x)y_i(x)dx=\frac{2\sqrt2[1-(-1)^{i+1}]}{(i+1)^3\pi^3}.
$$

Consequently the requested expansion has

$$
\boxed{A=\frac{4\sqrt2}{\pi^3},\qquad c_i=\frac{1-(-1)^{i+1}}{2(i+1)^3}.}
$$

Equivalently $u=(8/\pi^3)\sum_{n\geq1,\ n\text{ odd}}\sin(n\pi x)/n^3$. In particular $c_1=0$: the first excited [eigenfunction](../../../../eigenfunction.md) $\sqrt2\sin(2\pi x)$ is antisymmetric about $1/2$, whereas the trial function is symmetric. Since $10-\pi^2>0$, the final ratio is exactly

$$
\boxed{\frac{c_1^2(\lambda_1-\lambda_0)}{\lambda_{\rm trial}-\lambda_0}=0.}
$$

The first nonzero correction is $c_2=1/27$, not $c_1$. Reindexing only the nonzero terms would change the meaning of the requested ratio and is not used here.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
