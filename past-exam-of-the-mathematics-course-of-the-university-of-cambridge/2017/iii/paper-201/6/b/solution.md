<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a deterministic $a\geq0$. By the [Strong Markov property](../../../../../../strong-markov-property.md) at the finite [Brownian first-passage time](../../../../../../brownian-first-passage-time.md) $H_a$, the process $\widetilde B_s=B_{H_a+s}-a$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) started at zero. Such a process takes positive values arbitrarily soon [almost surely](../../../../../../almost-sure-convergence.md): for every $\varepsilon>0$, the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) makes its maximum on $[0,\varepsilon]$ have the distribution of $|B_\varepsilon|$, so the probability that the maximum is zero is zero. Intersecting these [events](../../../../../../event.md) for $\varepsilon=1/n$ gives an infimum of positive-crossing times equal to zero. Therefore

$$
\boxed{T_a=H_a\quad\text{almost surely for each fixed }a\geq0.}
$$

The infimum defining the strict crossing time need not itself be a time when $B_t>a$; continuity gives $B_{T_a}=a$. The quantifier here is fixed-level [almost sure equality](../../../../../../almost-sure-equality.md), not [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md) as the level varies.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
