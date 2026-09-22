<h1 id="14b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [drift-removing substitution for a Dirichlet Sturm-Liouville problem](../../../../../../drift-removing-substitution-for-a-dirichlet-sturm-liouville-problem.md), $y=e^{-x}v$. Direct differentiation gives $\mathcal Ly=e^{-x}(-v''+v)$. The homogeneous boundary conditions become $v(0)=v(\pi)=0$, so the [eigenvalues](../../../../../../eigenvalue.md) and [eigenfunctions](../../../../../../eigenfunction.md) are

$$
\boxed{\lambda_n=n^2+1,\qquad y_n=e^{-x}\sin(nx),\quad n=1,2,\ldots.}
$$

The self-adjoint weighted form is

$$
\mathcal Ly=-e^{-2x}(e^{2x}y')',\qquad
-(e^{2x}y')'=\lambda e^{2x}y.
$$

Thus the weight and leading coefficient are both $e^{2x}$. The [orthogonality of Sturm-Liouville eigenfunctions](../../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) reads

$$
\int_0^\pi e^{2x}y_ny_m\,dx=\frac\pi2\delta_{nm}.
$$

After multiplying the forcing equation by $e^x$, it becomes $-v''+v=x$. Expanding $x$ in the sine series of part (i) and dividing by $n^2+1$ gives

$$
\boxed{y(x)=2e^{-x}\sum_{n=1}^\infty
\frac{(-1)^{n+1}\sin(nx)}{n(n^2+1)}.}
$$

Every term satisfies the endpoint conditions. As a check, solving the transformed ODE directly gives $v=x-\pi\sinh x/\sinh\pi$, which has the same coefficients and forcing.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14B](../../14b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
