<h1 id="b/8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the constraint as $c(x)=1-x^Tx\geq0$ and its multiplier as $y\geq0$. The [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md) become

$$
\boxed{(A+yI)x=0,\qquad\|x\|_2\leq1,\qquad y\geq0,\qquad y(1-\|x\|_2^2)=0.}
$$

If $A$ is positive definite, $A+yI$ is positive definite for every $y\geq0$, so $\boxed{x=0,\ y=0}$ is the only critical point.

For indefinite $A$, the origin remains a critical point, contrary to an unqualified reading of the question. Every nonzero critical point is an [eigenvector](../../../../../eigenvector.md) with $\boxed{Ax=-yx}$, so its eigenvalue is nonpositive. A negative-eigenvalue vector must lie on the unit sphere, with multiplier equal to the negative of that eigenvalue. A nonzero vector in $\ker A$ may have any norm at most one and has multiplier zero. Positive-eigenvalue directions do not satisfy the multiplier sign condition. These first-order critical points include saddles; the global minimum selects a unit vector in the lowest-eigenvalue eigenspace.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
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
