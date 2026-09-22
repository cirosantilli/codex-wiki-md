<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce a free scalar $t$. The [epigraph](../../../../../../epigraph.md) reformulation is the [linear program](../../../../../../linear-programming.md)

$$
\min_{x\in\mathbb R^n,\,t\in\mathbb R}t\qquad\text{subject to}\qquad a_i^Tx+b_i\leq t\quad(1\leq i\leq n).
$$

For each fixed $x$, the smallest feasible $t$ equals the maximum of the affine expressions, so the reformulation preserves the optimum.

Associate nonnegative multipliers $y_i$ with these inequalities. Its [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
L(x,t,y)=\left(1-\sum_i y_i\right)t+\left(\sum_i y_i a_i\right)^Tx+\sum_i y_i b_i.
$$

Because $x$ and $t$ are unrestricted, the infimum is finite precisely when the coefficients of both vanish. Therefore the [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) is

$$
\boxed{\max_y\sum_i b_i y_i\qquad\text{subject to}\qquad\sum_i y_i a_i=0,\quad\sum_i y_i=1,\quad y_i\geq0.}
$$

A feasible dual vector is a [convex combination](../../../../../../convex-combination.md) of the slopes whose mean slope is zero. It gives a constant lower bound on the maximum of the affine functions. The primal is always feasible, by taking $x=0$ and sufficiently large $t$. If it has a finite optimum, [linear programming duality](../../../../../../linear-programming-duality.md) gives attainment and equality with this dual; otherwise the dual is infeasible and the primal is unbounded below.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
