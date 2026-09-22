<h1 id="b/7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First derive the standard consequence of [König theorem for cardinal numbers](../../../../../konig-s-theorem-set-theory.md) that every infinite [cardinal](../../../../../cardinal-number-split.md) $\rho$ satisfies

$$
\rho^{\operatorname{cf}(\rho)}>\rho.
$$

Let $\theta=\operatorname{cf}(\rho)$ and take [cofinal](../../../../../cofinal-subset.md) [ordinals](../../../../../ordinal-split.md) $\alpha_i<\rho$, $i<\theta$. Put $\rho_i=\max(1,|\alpha_i|)<\rho$. Their sum is $\rho$: it is at least the size of the union of the [cofinal](../../../../../cofinal-subset.md) [ordinals](../../../../../ordinal-split.md) and at most $\rho\cdot\theta=\rho$. Choose the next larger [cardinal](../../../../../cardinal-number-split.md) $\rho_i^+\leq\rho$. [König theorem for cardinal numbers](../../../../../konig-s-theorem-set-theory.md) gives

$$
\rho=\sum_{i<\theta}\rho_i<\prod_{i<\theta}\rho_i^+\leq\rho^\theta.
$$

This also covers $\rho=\aleph_0$, using finite [cardinals](../../../../../cardinal-number-split.md) and their next larger finite [cardinals](../../../../../cardinal-number-split.md).

Suppose $\lambda=\kappa^\mu$ with both $\kappa,\mu$ infinite. Infinite [cardinal](../../../../../cardinal-number-split.md) multiplication gives

$$
\lambda^\mu=(\kappa^\mu)^\mu=\kappa^{\mu\cdot\mu}=\lambda.
$$

If $\operatorname{cf}(\lambda)\leq\mu$, monotonicity of exponentiation would contradict the preceding strict inequality for $\rho=\lambda$. Thus $\operatorname{cf}(\lambda)>\mu\geq\aleph_0$. This direction does not require [GCH](../../../../../generalized-continuum-hypothesis.md).

Conversely assume [GCH](../../../../../generalized-continuum-hypothesis.md) and $\operatorname{cf}(\lambda)>\aleph_0$. Every function $\omega\to\lambda$ has bounded range. For each infinite [cardinal](../../../../../cardinal-number-split.md) $\nu<\lambda$, [GCH](../../../../../generalized-continuum-hypothesis.md) gives

$$
\nu^{\aleph_0}\leq(2^\nu)^{\aleph_0}=2^{\nu\cdot\aleph_0}=2^\nu=\nu^+\leq\lambda.
$$

Finite bounded ranges are also covered by the bound $\aleph_0^{\aleph_0}\leq\aleph_1\leq\lambda$. Counting functions according to an [ordinal](../../../../../ordinal-split.md) bound on their range now gives $\lambda^{\aleph_0}\leq\lambda\cdot\lambda=\lambda$. Constant functions give the reverse inequality. Therefore

$$
\boxed{\lambda=\lambda^{\aleph_0},}
$$

which is the required representation with $\kappa=\lambda$, $\mu=\aleph_0$. This proves both directions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
