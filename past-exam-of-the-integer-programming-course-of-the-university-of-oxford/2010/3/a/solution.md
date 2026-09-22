<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The retained [integer](../../../../integer-split.md) assignment constraints have only two feasible matrices,

$$
D=\begin{pmatrix}1&0\\0&1\end{pmatrix},\qquad O=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Their $(a\cdot x,b\cdot x,c\cdot x)$ totals are $(4,5,10)$ and $(3,6,8)$ respectively. For nonnegative [Lagrange multipliers](../../../../lagrange-multiplier.md) $\lambda,\mu$, add $\lambda(3.5-a\cdot x)+\mu(5.5-b\cdot x)$ to the maximization objective. Each [feasible point](../../../../feasible-point.md) gains a nonnegative amount, so maximizing over the retained assignment set gives an [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md):

$$
\theta(\lambda,\mu)=\max\left\{10-\frac\lambda2+\frac\mu2,\quad8+\frac\lambda2-\frac\mu2\right\}.
$$

The [Lagrangian dual problem](../../../../lagrangian-dual-problem.md) minimizes this convex piecewise-linear function over $\lambda,\mu\geq0$. Put $d=\lambda-\mu$; every real $d$ can occur. The two affine terms average to nine, so their maximum is at least nine, with equality exactly when $d=2$. Thus

$$
\boxed{\min_{\lambda,\mu\geq0}\theta=9,\qquad(\lambda,\mu)=(2+t,t),\quad t\geq0.}
$$

Neither [integer](../../../../integer-split.md) assignment satisfies both side constraints: $D$ violates the $a$ bound and $O$ the $b$ bound. The finite dual bound is therefore not evidence that the [integer](../../../../integer-split.md) primal is feasible. The following part shows why this [Lagrangian relaxation of an assignment with side constraints](../../../../lagrangian-relaxation-of-an-assignment-with-side-constraints.md) has a finite value anyway.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
