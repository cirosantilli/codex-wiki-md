<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mu$ be the [mutation](../../../../../../mutation.md) rate per chromosomal segment per generation, and use the population-scaled parameter $\theta=4N_e\mu$. In $2N_e$-generation coalescent units, [mutations](../../../../../../mutation.md) occur on each ancestral lineage at rate $\theta/2$. Independent [mutations](../../../../../../mutation.md) on all branches of a given [phylogenetic tree](../../../../../../phylogenetic-tree.md) superpose to give a [Poisson distribution](../../../../../../poisson-distribution.md) with [mean](../../../../../../expected-value.md) $\theta L/2$.

Under the [infinite sites mutation model](../../../../../../infinite-sites-mutation-model.md), each [mutation](../../../../../../mutation.md) occurs at a distinct position, and every [mutation](../../../../../../mutation.md) below the sample's common ancestor separates a nonempty proper subset of sampled [chromosomes](../../../../../../chromosome.md) from the remainder. Thus the [mutation](../../../../../../mutation.md) count is exactly the [segregating site](../../../../../../segregating-site.md) count, giving

$$
\boxed{S\mid L,\theta\sim\operatorname{Poisson}\!\left(\frac{\theta L}{2}\right).}
$$

By the [law of total expectation](../../../../../../law-of-total-expectation.md) and the previous branch-length formula,

$$
\boxed{E[S\mid\theta]=E\!\left[\frac{\theta L}{2}\right]=\theta a_n.}
$$

This also gives the [Watterson estimator](../../../../../../watterson-estimator.md) $S/a_n$ as an unbiased moment estimator of $\theta$. Here all sample [segregating sites](../../../../../../segregating-site.md) are counted, including singletons; filtering sites by a minimum sample frequency or by external [SNP](../../../../../../single-nucleotide-polymorphism.md) discovery would introduce [genetic-study ascertainment](../../../../../../genetic-study-ascertainment.md) and change this calculation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
