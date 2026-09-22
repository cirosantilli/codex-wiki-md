# Support-preserving right-hand-side changes in linear programming

↑ **Parent:** [Complementary slackness](complementary-slackness.md)

For the [linear program](linear-programming-split.md) maximizing $c^Tx$ subject to $Ax=b$, $x\geq0$, let $x^*$ be optimal and let $y^*$ be an optimal [dual linear program](dual-linear-program.md) solution. [Complementary slackness](complementary-slackness.md) makes $A_j^Ty^*=c_j$ on every positive coordinate of $x^*$. Any nonnegative $\widehat x$ supported on those coordinates therefore has

$$
c^T\widehat x=(y^*)^TA\widehat x.
$$

The same $y^*$ is dual feasible when the right-hand side is changed to $\widehat b=A\widehat x$. Equality of feasible objectives and [weak duality](weak-duality.md) prove optimality of $\widehat x$ for that modified problem.

There is also a direct primal proof. If $z\geq0$ had $Az=A\widehat x$ and $c^Tz>c^T\widehat x$, then $x^*+\varepsilon(z-\widehat x)$ would remain feasible and nonnegative for sufficiently small $\varepsilon>0$. On zero coordinates of $x^*$, support inclusion makes its perturbation nonnegative; on positive coordinates, smallness preserves positivity. Its objective would improve, contradicting optimality of $x^*$.

## ↑ Ancestors (7)

1. [Complementary slackness](complementary-slackness.md)
2. [Linear programming duality](linear-programming-duality.md)
3. [Linear programming](linear-programming-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/t/1/b/solution.md)
