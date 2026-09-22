<h1 id="27k/solution">Solution</h1>

↑ **Parent:** [27K](../27k.md)

A [renewal-reward process](../../../../../renewal-reward-process.md) consists of i.i.d. regenerative cycles $(\xi_n,R_n)$, where $\xi_n>0$ is the $n$th cycle length and $R_n$ is the reward accumulated during that cycle. If $0<\mathbb E\xi_1<\infty$ and $\mathbb E|R_1|<\infty$, the [renewal-reward theorem](../../../../../renewal-reward-theorem.md) states that the cumulative reward $Z(t)$ satisfies

$$
\frac{Z(t)}t\longrightarrow\frac{\mathbb E R_1}{\mathbb E\xi_1}
$$

almost surely, with the usual negligible-remainder condition for an unfinished cycle.

For the machine, let $X\sim\operatorname{Exp}(\lambda)$ be its working lifetime after a repair. The next repair occurs at the first inspection following failure, so one repair-to-repair cycle has length

$$
\xi=m\left\lceil\frac Xm\right\rceil,
$$

while its working-time reward is $R=X$. Since an [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$ has mean $1/\lambda$,

$$
\mathbb ER=\frac1\lambda.
$$

By the [tail-sum formula](../../../../../tail-sum-formula.md) for the positive integer-valued variable $\lceil X/m\rceil$,

$$
\mathbb E\left\lceil\frac Xm\right\rceil
=\sum_{k=0}^{\infty}\mathbb P(X>km)
=\sum_{k=0}^{\infty}e^{-\lambda km}
=\frac1{1-e^{-\lambda m}}.
$$

Therefore

$$
\mathbb E\xi=\frac{m}{1-e^{-\lambda m}},
$$

and the [long-run proportion of time for which the machine is working](../../../../../long-run-availability-under-periodic-inspection.md) is

$$
\boxed{\frac{\mathbb ER}{\mathbb E\xi}
=\frac{1-e^{-\lambda m}}{\lambda m}}.
$$

## ↑ Ancestors (10)

1. [27K](../27k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
