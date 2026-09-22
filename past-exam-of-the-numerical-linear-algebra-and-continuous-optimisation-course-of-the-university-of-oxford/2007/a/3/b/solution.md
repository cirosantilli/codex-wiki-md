<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For homogeneous error boundary values, the tensor-product sine vectors $U_{j,k}=\sin(r\pi jh)\sin(s\pi kh)$ form a basis. The sine addition formula gives $U_{j+1,k}+U_{j-1,k}=2\cos(r\pi h)U_{j,k}$, and similarly in the other coordinate. Hence the five-point matrix has

$$
\boxed{\lambda_{r,s}=4-2\cos(r\pi h)-2\cos(s\pi h),\qquad r,s=1,\ldots,n.}
$$

There is a printing error in the displayed iteration. Taken literally, its error multiplier is $1/20-(2/5)(\cos(r\pi h)+\cos(s\pi h))$, and its fixed-point equation is $(19/4)U_{j,k}+\sum_{\mathrm{neighbors}}U=h^2f_{j,k}$, rather than the stated Poisson equation. Thus the printed affine update cannot be used as a consistent relaxation for this system.

The intended [weighted Jacobi iteration](../../../../../weighted-jacobi-method.md) with $\omega=4/5$ is

$$
\boxed{U_{j,k}^{\mathrm{new}}=\frac15U_{j,k}^{\mathrm{old}}+\frac15\sum_{\mathrm{neighbors}}U^{\mathrm{old}}+\frac15h^2f_{j,k}.}
$$

Its [iteration matrix](../../../../../iteration-matrix.md) is $I-(\omega/4)A$, whose mode multiplier is

$$
\boxed{\mu_{r,s}=1-\frac45+\frac25\bigl(\cos(r\pi h)+\cos(s\pi h)\bigr).}
$$

If at least one of the two cosines is negative, their sum lies strictly between $-2$ and $1$, so $-3/5<\mu_{r,s}<3/5$. Thus every such high-frequency mode contracts by at most $\boxed{3/5}$ per sweep, uniformly in grid spacing. This [weighted Jacobi smoothing bound for the square Poisson problem](../../../../../weighted-jacobi-smoothing-bound-for-the-square-poisson-problem.md) justifies the corrected method as a smoother. The literal printed update also damps modes, but toward the wrong fixed-point equation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
