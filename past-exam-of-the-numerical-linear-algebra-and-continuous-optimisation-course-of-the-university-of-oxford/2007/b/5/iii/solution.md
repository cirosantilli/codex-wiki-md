<h1 id="b/5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The global optimality conditions for a quadratic [trust-region subproblem](../../../../../trust-region-subproblem.md) with Hessian $B$ are: for some $\lambda\geq0$,

$$
(B+\lambda I)s=-g,\qquad B+\lambda I\succeq0,\qquad\|s\|_2\leq\Delta,\qquad\lambda(\|s\|_2-\Delta)=0.
$$

Here $B=I$, so the shifted matrix is positive definite. If $\|g\|_2\leq\Delta$, choose $\lambda=0$ and $s=-g$. If $\|g\|_2>\Delta$, the active boundary gives $s=-g/(1+\lambda)$ and $1+\lambda=\|g\|_2/\Delta$. Hence

$$
\boxed{s_*=-g\quad(\|g\|_2\leq\Delta),\qquad s_*=-\Delta g/\|g\|_2\quad(\|g\|_2>\Delta).}
$$

This is exactly the [Cauchy point](../../../../../cauchy-point.md). Because the model is strictly convex, it is the unique global minimizer, including $s_*=0$ when $g=0$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
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
