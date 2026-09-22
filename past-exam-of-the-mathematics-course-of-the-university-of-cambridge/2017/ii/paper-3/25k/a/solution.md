<h1 id="25k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a neutral [Moran model](../../../../../../moran-process.md), a population has $N$ labelled individuals; reproduction copies one individual's type to a uniformly chosen other individual, keeping population size fixed. One convenient time convention puts independent rate-$1/2$ Poisson arrows on each ordered pair of distinct individuals. Backwards in time, two sampled ancestral lineages merge whenever one copies the other, at total rate $1$ per unordered pair. In the convention where each individual reproduces at rate $1$, this pair rate is $2/(N-1)$ if the parent cannot replace itself, and time must be rescaled accordingly.

[Kingman's coalescent](../../../../../../kingman-s-coalescent.md) on $n$ labels is the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) on partitions of $\{1,\ldots,n\}$, initially all singleton blocks, in which each pair of distinct blocks merges at rate $1$. With $j$ blocks, the waiting time is exponential of rate $\binom j2$, and the merging pair is uniform. [Kingman's infinite coalescent](../../../../../../kingman-s-infinite-coalescent.md) is the consistent partition process on $\mathbb N$ whose restriction to each finite label [set](../../../../../../set-split.md) has this law; consistency and the extension theorem construct it. These time conventions are part of the definition.

Let $B_t^{(n)}$ be the number of blocks in the first $n$ labels. The expected time to reach at most $m$ blocks is

$$
 \mathbb E T_m^{(n)}=\sum_{j=m+1}^n\binom j2^{-1}=2\left(\frac1m-\frac1n\right)\leq\frac2m.
$$

[Markov inequality](../../../../../../markov-inequality.md) gives $\mathbb P(B_t^{(n)}>m)\leq2/(mt)$. As $n$ increases these counts increase to the total number of infinite-coalescent blocks, so the same bound holds for that number. Letting $m\to\infty$ shows it is finite [almost surely](../../../../../../almost-sure-convergence.md) for each $t>0$. Apply this simultaneously to positive rational times; monotonicity of the block count then covers every positive real time. Hence **[Kingman's infinite coalescent](../../../../../../kingman-s-infinite-coalescent.md) comes down from infinity [almost surely](../../../../../../almost-sure-convergence.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
