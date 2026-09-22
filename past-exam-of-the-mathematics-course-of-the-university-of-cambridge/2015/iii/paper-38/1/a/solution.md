<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [maximization problem](../../../../../../maximization-problem.md) with $g_i(u)\leq0$ and $h_j(u)=0$, use the [optimization Lagrangian](../../../../../../optimization-lagrangian.md)

$$
L(u,\lambda,\mu)=f(u)-\sum_i\lambda_i g_i(u)-\sum_j\mu_jh_j(u),\qquad \lambda_i\geq0.
$$

The [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) says: if $u^*$ is feasible, $u^*$ globally maximizes $L(\cdot,\lambda^*,\mu^*)$ over its original domain, and [complementary slackness](../../../../../../complementary-slackness.md) holds, $\lambda_i^*g_i(u^*)=0$, then $u^*$ globally maximizes $f$ over the feasible set. Equality [Lagrange multipliers](../../../../../../lagrange-multiplier.md) have no sign restriction. For every feasible $u$,

$$
f(u)\leq L(u,\lambda^*,\mu^*)\leq L(u^*,\lambda^*,\mu^*)=f(u^*),
$$

which proves the theorem.

For a [minimization problem](../../../../../../minimization-problem.md), reverse the signs in the [optimization Lagrangian](../../../../../../optimization-lagrangian.md): take $L=f+\sum_i\lambda_i g_i+\sum_j\mu_jh_j$, with $\lambda_i\geq0$. If a feasible $u^*$ globally minimizes this [optimization Lagrangian](../../../../../../optimization-lagrangian.md) and satisfies [complementary slackness](../../../../../../complementary-slackness.md), then

$$
f(u)\geq L(u,\lambda^*,\mu^*)\geq L(u^*,\lambda^*,\mu^*)=f(u^*).
$$

**The hypothesis is a global extremum of the Lagrangian.** Merely solving its stationarity equations is insufficient; no convexity assumption is needed when the global extremum itself has been proved.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
