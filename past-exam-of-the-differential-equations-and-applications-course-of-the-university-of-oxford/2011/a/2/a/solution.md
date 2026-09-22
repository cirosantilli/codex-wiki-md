<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $t=\log x$ and $Y(t)=y(e^t)$. Then $xy''+y'=Y''/x$, so the [eigenvalue problem](../../../../../eigenvalue-problem.md) reduces to

$$
Y''+(4+\lambda)Y=0,\qquad Y(0)=Y(\pi)=0.
$$

A nonzero [Dirichlet eigenfunction](../../../../../dirichlet-eigenfunction.md) therefore has $4+\lambda=n^2$ for an integer $n\geq1$. The complete family is

$$
\boxed{\lambda_n=n^2-4,\qquad y_n(x)=\sin(n\log x),\qquad n=1,2,\ldots.}
$$

The alternatives $4+\lambda\leq0$ give only the zero solution under both endpoint conditions.

The operator itself is **self-adjoint with the given unweighted inner product**, on the usual regular Dirichlet domain. Indeed $My=(xy')'+4y/x$, and [integration by parts](../../../../../integration-by-parts.md) gives

$$
\langle f,Mg\rangle-\langle Mf,g\rangle=[x(fg'-f'g)]_1^{e^\pi}=0
$$

for functions satisfying the endpoint conditions. This is a regular [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) with positive leading coefficient $x$, whose Dirichlet realization is self-adjoint. The displayed generalized eigenproblem contains the additional weight $1/x$; its eigenfunctions are accordingly [orthogonal](../../../../../orthogonal-vectors.md) with respect to $\int fg/x$, which is separate from the self-adjointness assertion about $M$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
