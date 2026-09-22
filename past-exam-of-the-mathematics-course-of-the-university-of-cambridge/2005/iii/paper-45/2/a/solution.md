<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [kinship coefficient](../../../../../../kinship-coefficient.md) $\phi_{XY}$ is the [probability](../../../../../../probability.md) that a randomly selected [allele](../../../../../../allele.md) copy from individual $X$ and an independently selected copy from individual $Y$ at the same [genetic locus](../../../../../../genetic-locus.md) are [identical by descent](../../../../../../identity-by-descent.md). The sampling is of gene copies, not of whole [genotypes](../../../../../../genotype.md). For a noninbred individual $X$, sampling its two copies with replacement gives $\phi_{XX}=1/2$; in general $\phi_{XX}=(1+F_X)/2$, where $F_X$ is its [inbreeding coefficient](../../../../../../inbreeding-coefficient.md).

For two [full siblings](../../../../../../full-sibling.md) in an [outbred pedigree](../../../../../../outbred-pedigree.md), the two sampled copies are both paternal with [probability](../../../../../../probability.md) $1/4$, both maternal with [probability](../../../../../../probability.md) $1/4$, and of different parental origin with [probability](../../../../../../probability.md) $1/2$. Given that both are paternal, their independent [Mendelian segregation](../../../../../../mendelian-segregation.md) transmissions select the same paternal ancestral copy with [probability](../../../../../../probability.md) $1/2$; likewise for both maternal. The different-parent case cannot be [identical by descent](../../../../../../identity-by-descent.md) when the parents are unrelated. Therefore

$$
\boxed{\phi_{\mathrm{sib}}=\frac14\cdot\frac12+\frac14\cdot\frac12+\frac12\cdot0=\frac14.}
$$

Equivalently, conditional on an IBD-sharing count $J$, the chance that the two random copies match is $J/4$, so $\phi_{\mathrm{sib}}=E[J]/4=1/4$. The expected shared proportion $E[J/2]=1/2$ and the usual additive relationship coefficient $2\phi=1/2$ are twice this [kinship coefficient](../../../../../../kinship-coefficient.md); confusing these conventions would double the subsequent [inbreeding coefficient](../../../../../../inbreeding-coefficient.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
