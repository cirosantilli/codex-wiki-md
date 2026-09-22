<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

The [Lagrange sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) for maximizing $f$ subject to $g_i\geq0$ and $h_j=0$ states that if a feasible point $x^*$ and multipliers $\lambda_i\geq0,\mu_j$ satisfy complementary slackness and $x^*$ globally maximizes the [Lagrangian function in constrained optimization](../../../../../lagrangian-function-in-constrained-optimization.md)

$$
L(x)=f(x)+\sum_i\lambda_i g_i(x)+\sum_j\mu_jh_j(x),
$$

then $x^*$ globally maximizes $f$ on the feasible set.

For the equality constraint, take

$$
L=\log x+\log y+\log z+\lambda(1-x^2-y^2-z^2).
$$

The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations give

$$
\frac1x=2\lambda x,
\qquad
\frac1y=2\lambda y,
\qquad
\frac1z=2\lambda z,
$$

so positivity and the constraint imply

$$
x=y=z=\frac1{\sqrt3},
\qquad \lambda=\frac32.
$$

For this multiplier, $L$ is a [strictly concave function](../../../../../strictly-concave-function.md) on the positive octant and its stationary point is its unique global maximum. The sufficiency theorem therefore proves that the constrained maximum is

$$
\boxed{\max\log(xyz)=\log\frac1{3\sqrt3}=-\frac32\log3}.
$$

For $x^2+y^2+z^2\leq1$, use $g=1-x^2-y^2-z^2$. The same point and multiplier satisfy feasibility, stationarity, $\lambda\geq0$, and [complementary slackness](../../../../../complementary-slackness.md), and they again globally maximize the Lagrangian. Hence the answer is unchanged. Equivalently, any point with strict inequality can be radially scaled outward, increasing all three positive coordinates and therefore increasing $\log(xyz)$.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
