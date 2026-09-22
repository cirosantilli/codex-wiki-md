<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R[y]=F[y]/G[y]$, where $G[y]>0$ for a nonzero admissible real function. Writing $\lambda=R[y]$, its first variation is

$$
\delta R=\frac2G\left\{[py'\delta y]_\alpha^\beta+\int_\alpha^\beta[-(py')'+qy-\lambda wy]\delta y\,dx\right\}.
$$

Choose [boundary conditions](../../../../../boundary-condition.md) making the boundary term vanish, for example homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), or a corresponding mixed pair. Arbitrary interior variations then give the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md)

$$
\boxed{-(py')'+qy=\lambda wy.}
$$

Multiplying this equation by $y$ and integrating by parts, with $[pyy']_\alpha^\beta=0$, yields

$$
\boxed{\lambda=\frac{\int_\alpha^\beta[p(y')^2+qy^2]dx}{\int_\alpha^\beta wy^2dx}=R[y].}
$$

Thus [eigenfunctions](../../../../../eigenfunction.md) are stationary directions of the quotient. The lowest [eigenvalue](../../../../../eigenvalue.md) is its global minimum; higher [eigenfunctions](../../../../../eigenfunction.md) need not be unrestricted maxima or minima. General Robin [boundary conditions](../../../../../boundary-condition.md) require including their boundary energy in the quotient unless the displayed endpoint products also vanish.

The [Rayleigh-Ritz method](../../../../../rayleigh-ritz-method.md) chooses admissible trial functions depending on finitely many coefficients and minimizes this quotient over them. Expansion in a complete orthonormal basis with weight $w$ shows $R[y]\geq\lambda_0$, so the trial minimum is an upper bound on the true lowest [eigenvalue](../../../../../eigenvalue.md). In a finite basis, the minimization becomes a [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) for the stiffness and weighted mass [matrices](../../../../../matrix.md). Enlarging the trial space can only lower or preserve this upper bound.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
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
