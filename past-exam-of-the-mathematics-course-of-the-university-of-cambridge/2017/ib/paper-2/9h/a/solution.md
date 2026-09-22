<h1 id="9h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a vector equality constraint, take the [Lagrangian function in constrained optimization](../../../../../../lagrangian-function-in-constrained-optimization.md)

$$
\boxed{L(x,\lambda)=f(x)+\lambda^T(b-g(x)),\qquad x\in X,\quad\lambda\in\mathbb R^m.}
$$

The sign of the multiplier is a convention; equality multipliers are unrestricted. The [Lagrange sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) says that if $x^*\in X$ is feasible and, for some $\lambda^*$, globally minimizes $L(\cdot,\lambda^*)$ over $X$, then $x^*$ globally minimizes the constrained objective.

Indeed for any feasible $x$, $f(x)=L(x,\lambda^*)\ge L(x^*,\lambda^*)=f(x^*)$. Thus $\boxed{x^*\text{ is a global primal minimizer}}$. The theorem requires a global Lagrangian minimum, not merely a stationary point. It needs neither differentiability nor convexity when stated in this form; those hypotheses can be used separately to establish the required minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9H](../../9h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
