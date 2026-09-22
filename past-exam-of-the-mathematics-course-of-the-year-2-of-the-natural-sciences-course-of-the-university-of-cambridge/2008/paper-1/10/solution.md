<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

For nonzero $y$ with $G[y]>0$, the [first variation](../../../../first-variation.md) of the [Rayleigh quotient](../../../../rayleigh-quotient.md) under $y\mapsto y+\varepsilon h$ is

$$
\delta\Lambda=\frac2{G[y]}\left\{\int_a^b[-(py')'+qy-\Lambda wy]h\,dx+[py'h]_a^b\right\}.
$$

Choose fixed admissible homogeneous [boundary conditions](../../../../boundary-condition.md) that make the variation boundary term vanish, such as zero endpoint values or zero endpoint derivatives. Compactly supported $h$ then show that a stationary function satisfies the [Sturm-Liouville equation](../../../../sturm-liouville-equation.md) with $\lambda=\Lambda[y]$. Conversely an [eigenfunction](../../../../eigenfunction.md) satisfying those admissible conditions makes the variation zero. Multiplying its differential equation by $y$ and integrating by parts gives

$$
F[y]-[pyy']_a^b=\lambda G[y],
$$

so the stipulated energy boundary term yields $\Lambda[y]=\lambda$. The displayed energy condition alone is not a full specification of the admissible variations; it must be paired with boundary conditions for this variational equivalence.

For the final Dirichlet problem take the trial function $y=\sin x$, with $p=1,q=0,w=x$. Then

$$
\int_0^\pi y'^2dx=\frac\pi2,\qquad \int_0^\pi xy^2dx=\frac{\pi^2}4,
\qquad\boxed{\lambda_e=\frac2\pi\approx0.63662.}
$$

The [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md) makes this an upper bound for the lowest [eigenvalue](../../../../eigenvalue.md). It is strictly above the true value: equality would require $\sin x$ itself to be a lowest [eigenfunction](../../../../eigenfunction.md), but $y''+\lambda xy=(-1+\lambda x)\sin x$ cannot vanish throughout $(0,\pi)$ for a constant $\lambda$. Therefore

$$
\boxed{\lambda_e-\lambda_t>0.}
$$

Although the weight vanishes at the left endpoint, it is positive in the interior and its weighted quadratic norm is positive for every nonzero admissible continuous function; this does not obstruct the stated Dirichlet variational comparison.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
