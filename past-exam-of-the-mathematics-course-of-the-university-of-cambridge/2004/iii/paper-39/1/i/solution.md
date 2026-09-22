<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

During the epoch with $j$ ancestral lineages, [Kingman's coalescent](../../../../../../kingman-s-coalescent.md) has waiting time $T_j\sim\operatorname{Exp}(\binom j2)$. In the stated time units, each lineage accumulates [mutations](../../../../../../mutation.md) at rate $Nu=\theta/2$, so the [mutation count on a neutral coalescent tree](../../../../../../mutation-count-on-a-neutral-coalescent-tree.md) decomposes as

$$
S=\sum_{j=2}^nY_j,\qquad Y_j\mid T_j\sim\operatorname{Poisson}\left(\frac{j\theta T_j}{2}\right).
$$

The [law of total expectation](../../../../../../law-of-total-expectation.md) and the mean of an [exponential distribution](../../../../../../exponential-distribution.md) give $\mathbb EY_j=(j\theta/2)/\binom j2=\theta/(j-1)$. Therefore

$$
\boxed{\mathbb ES=\theta H_{n-1},\qquad H_{n-1}=\sum_{i=1}^{n-1}\frac1i.}
$$

This calculation counts mutation events. Equating the count with observed [segregating sites](../../../../../../segregating-site.md) additionally uses the [infinite sites mutation model](../../../../../../infinite-sites-mutation-model.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
