<h1 id="a/2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $v=Ly$ as

$$
v(x)=\cos x\int_x^\pi\sin t\,y(t)\,dt+\sin x\int_0^x\cos t\,y(t)\,dt.
$$

Differentiating twice, the moving-limit terms cancel at first order and yield $\boxed{v''+v=y}$ at second order. Also $v'(0)=0$ and $v(\pi)=0$. Thus this [integral operator](../../../../../../integral-operator.md) is the inverse of $D^2+1$ with mixed [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) and [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md).

For $\kappa_n=n+1/2$, $y_n(x)=\cos(\kappa_nx)$ satisfies those conditions and $(D^2+1)y_n=(1-\kappa_n^2)y_n$. The corresponding mixed homogeneous equation has no nonzero solution, so uniqueness gives

$$
\boxed{Ly_n=\lambda_ny_n,\qquad\lambda_n=\frac1{1-\kappa_n^2}=-\frac4{4n^2+4n-3}.}
$$

This verifies the asserted [eigenvalues](../../../../../../eigenvalue.md) and [eigenfunctions](../../../../../../eigenfunction.md) for every $n\geq0$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
