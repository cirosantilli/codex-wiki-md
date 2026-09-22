<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Multiply the original equation by $p(x)=\exp(\int^xu(s)ds)>0$. Since $p'=up$, it becomes $(py')'+qy+\lambda ry=0$ with $q=pv$, $r=pw>0$. This is [Sturm-Liouville form](../../../../sturm-liouville-form.md). For two real [eigenfunctions](../../../../eigenfunction.md), multiply the equation for $y_n$ by $y_m$, subtract the equation for $y_m$ multiplied by $y_n$, and integrate. The [Lagrange identity for a Sturm-Liouville operator](../../../../lagrange-identity-for-a-sturm-liouville-operator.md) gives

$$
(\lambda_m-\lambda_n)\int_a^br\,y_my_n\,dx=[p(y_my_n'-y_ny_m')]_a^b.
$$

Each separated homogeneous boundary condition makes the corresponding determinant zero, provided its pair of coefficients is not both zero. For distinct [eigenvalues](../../../../eigenvalue.md), this proves the [orthogonality of Sturm-Liouville eigenfunctions](../../../../orthogonality-of-sturm-liouville-eigenfunctions.md).

For the constant drift, the [drift-removing substitution for a Dirichlet Sturm-Liouville problem](../../../../drift-removing-substitution-for-a-dirichlet-sturm-liouville-problem.md) is $y=e^{-\alpha x}v$. It reduces the equation to $v''+\lambda v=0$ with $v(0)=v(\pi)=0$. Nonzero solutions occur exactly at

$$
\boxed{\lambda_n=n^2,\qquad y_n=e^{-\alpha x}\sin nx,\quad n=1,2,\ldots.}
$$

The zero and negative values give only the zero solution under both endpoint conditions. The self-adjoint expression is $(e^{2\alpha x}y')'+\alpha^2e^{2\alpha x}y+\lambda e^{2\alpha x}y=0$. Hence the weight is $r=e^{2\alpha x}$, and for the displayed normalization,

$$
\boxed{\int_0^\pi e^{2\alpha x}y_my_n\,dx=\frac\pi2\delta_{mn}.}
$$

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
