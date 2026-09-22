<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use standard diploid coalescent time units of $2N_e$ generations, where $N_e$ is the fixed [effective population size](../../../../../../effective-population-size.md), and take $n\ge2$. In the neutral [Kingman's coalescent](../../../../../../kingman-s-coalescent.md), each unordered pair of ancestral lineages merges at rate one. With $j$ lineages, the next coalescence time therefore has an [exponential distribution](../../../../../../exponential-distribution.md) with rate

$$
\lambda_j=\binom j2=\frac{j(j-1)}2,\qquad E[T_j]=\frac{2}{j(j-1)}.
$$

The memoryless construction and the [Markov property](../../../../../../markov-property.md) make these epoch durations independent. During epoch $j$ there are $j$ branches, each of duration $T_j$, so the [total branch length of a neutral coalescent](../../../../../../total-branch-length-of-a-neutral-coalescent.md) is

$$
L=\sum_{j=2}^n jT_j.
$$

By linearity of [expectation](../../../../../../expected-value.md),

$$
\boxed{E[L]=\sum_{j=2}^n\frac{2}{j-1}=2\sum_{i=1}^{n-1}\frac1i=2a_n,\qquad a_n=\sum_{i=1}^{n-1}\frac1i.}
$$

The ancestral branch above the sample's most recent common ancestor is excluded: [mutations](../../../../../../mutation.md) there would be shared by all sampled [chromosomes](../../../../../../chromosome.md) and would not create [segregating sites](../../../../../../segregating-site.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
