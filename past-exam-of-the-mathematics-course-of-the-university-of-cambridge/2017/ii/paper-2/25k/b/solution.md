<h1 id="25k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the zero set $A=\{s\in[0,t]:g(s)=0\}$ is measurable, as is ensured by measurability of $g$. This is an implicit necessary hypothesis: for an arbitrary real function the printed [integral](../../../../../../integral.md) and event need not be measurable. Put $a=\int_0^t\mathbf1_A(s)\,ds$. Conditional on $N_t=n$, the [uniform order statistics](../../../../../../uniform-order-statistic.md) description makes the [probability](../../../../../../probability.md) of no jump in $A$ equal to $(1-a/t)^n$. Averaging over the [Poisson distribution](../../../../../../poisson-distribution.md) gives

$$
\mathbb P(0\notin\mathcal R(g)[0,t])
=e^{-\lambda t}\sum_{n=0}^\infty\frac{[\lambda t(1-a/t)]^n}{n!}=e^{-\lambda a}.
$$

Consequently

$$
\boxed{\mathbb P(0\in\mathcal R(g)[0,t])=1-\exp\left(-\lambda\int_0^t\mathbf1_{\{g(s)=0\}}\,ds\right).}
$$

In particular a measure-zero zero set is almost surely missed, despite possibly containing infinitely many points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25K](../../25k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
