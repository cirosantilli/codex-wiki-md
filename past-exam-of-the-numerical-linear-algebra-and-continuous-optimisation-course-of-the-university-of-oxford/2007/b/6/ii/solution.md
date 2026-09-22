<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [sequential quadratic programming](../../../../../sequential-quadratic-programming.md) step minimizes a quadratic local objective model while enforcing the first-order constraint expansion $c(x_k+s)\approx c_k+A_ks=0$. When the iterate and multipliers are close to a regular solution and $B_k$ approximates the Lagrangian Hessian, the resulting correction approximates a [Newton step](../../../../../newton-step.md) for the nonlinear [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md).

Full row rank of $A_k$ ensures that $A_ks=-c_k$ is solvable for every $c_k$ and that the multiplier of the quadratic subproblem is unique. A positive-definite $B_k$ makes the objective strictly convex and coercive on the affine feasible set, giving a unique global subproblem minimizer. In fact positivity on $\ker A_k$, rather than on every vector, is enough for uniqueness and boundedness on that set; full positive definiteness is a convenient stronger assumption.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
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
