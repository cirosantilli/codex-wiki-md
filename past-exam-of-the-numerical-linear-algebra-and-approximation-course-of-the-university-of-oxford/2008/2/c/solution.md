<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Order points along each $j$-line before moving to the next $k$-line. The splitting has

$$
M=\operatorname{diag}(T_n,\ldots,T_n),\qquad T_n=\operatorname{tridiag}(-1,4,-1),
$$

and $N$ couples the two neighboring $k$-lines. Factor $T_n$ once with the [Thomas algorithm](../../../../tridiagonal-matrix-algorithm.md); each iteration then needs $n$ tridiagonal solves and the neighboring-line right sides, costing $\boxed{O(n^2)}$ for $n^2$ unknowns. Known boundary values are moved to the right side; the error eigenmodes have homogeneous boundary values.

The [generalized eigenvalue problem](../../../../generalized-eigenvalue-problem.md) is

$$
U_{j,k+1}+U_{j,k-1}=\lambda(4U_{j,k}-U_{j+1,k}-U_{j-1,k}),
$$

with $U=0$ at the boundary indices. Put $\theta_r=r\pi/(n+1)$, $\theta_s=s\pi/(n+1)$. The sine addition formula gives $U_{j+1,k}+U_{j-1,k}=2\cos\theta_r\,U_{j,k}$ and the corresponding identity in $k$. Thus

$$
\boxed{\lambda_{r,s}=\frac{2\cos\theta_s}{4-2\cos\theta_r}=\frac{\cos\theta_s}{2-\cos\theta_r}.}
$$

These tensor-product sine vectors form a basis, so they give the whole spectrum. With $c=\cos(\pi/(n+1))\in[0,1)$,

$$
\boxed{\rho(M^{-1}N)=\frac{c}{2-c}<1.}
$$

The iteration therefore converges.

It is **not a uniformly effective multigrid smoother**. Take $r=1$ and $s=n$: the error is slowly varying along a line but highly oscillatory between lines, and its multiplier is $-c/(2-c)\to-1$ as the grid is refined. It changes sign at each step while retaining almost its full amplitude. This [line-Jacobi Fourier spectrum](../../../../line-jacobi-fourier-spectrum.md) distinguishes convergence on each fixed grid from the high-frequency damping needed by the [multigrid method](../../../../multigrid-method-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
