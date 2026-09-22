<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a minimization problem on a domain $D$, write the equality constraints as $h(x)=0$ and the inequality constraints as $g(x)\leq0$. Define the [optimization Lagrangian](../../../../../../optimization-lagrangian.md)

$$
L(x,\lambda,\mu)=f(x)+\lambda^T h(x)+\mu^Tg(x),\qquad \mu\geq0.
$$

The [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) states that a feasible $x^*$ is globally optimal if it globally minimizes $L(\cdot,\lambda^*,\mu^*)$ on $D$ for some multipliers with $\mu^*\geq0$ and satisfies [complementary slackness](../../../../../../complementary-slackness.md), $\mu_j^*g_j(x^*)=0$ for every $j$. Equality multipliers have unrestricted signs.

For any feasible $x$, the multiplier sign gives $L(x,\lambda^*,\mu^*)\leq f(x)$. Feasibility and [complementary slackness](../../../../../../complementary-slackness.md) at $x^*$ give $L(x^*,\lambda^*,\mu^*)=f(x^*)$. Hence

$$
\boxed{f(x)\geq L(x,\lambda^*,\mu^*)\geq L(x^*,\lambda^*,\mu^*)=f(x^*).}
$$

This proves sufficiency. **Global Lagrangian minimization, rather than stationarity alone, is the certificate.** No [convexity](../../../../../../convex-function.md) or constraint qualification is needed for this implication; [convexity](../../../../../../convex-function.md) is one way to verify the required global minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
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
