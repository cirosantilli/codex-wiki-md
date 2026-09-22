<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Under the original assumptions the extra affected child is impossible. A generation-3 woman can have at most one copy of the unique introduced disease [allele](../../../../../../allele.md), while an unrelated outside spouse has none. Their children cannot inherit two defective copies. Thus both linkage and no-linkage [likelihoods](../../../../../../likelihood-function.md) of the enlarged data are zero, and **the original single-entry model has no defined updated [LOD score](../../../../../../lod-score.md)**. At least one assumption must be relaxed: another introduced disease [allele](../../../../../../allele.md), a new mutation, a phenocopy, or the relationship of the outside spouse.

If the model is enlarged to allow an independent outside [genetic carrier](../../../../../../genetic-carrier.md), the reported extra information contains disease status but no new [genetic marker](../../../../../../genetic-marker.md) [genotypes](../../../../../../genotype.md). In the simple extension with fixed outside heterozygous-carrier [probability](../../../../../../probability.md) $c$, the old disease observations force both generation-2 family ancestors to be [genetic carriers](../../../../../../genetic-carrier.md). A further generation-3 sister inherits the disease copy with [probability](../../../../../../probability.md) $1/2$, independently of the existing offspring transmissions. Given that she and her spouse are [genetic carriers](../../../../../../genetic-carrier.md), exactly one of their three children is affected with [probability](../../../../../../probability.md)

$$
\binom31\frac14\left(\frac34\right)^2=\frac{27}{64}.
$$

The additional [phenotype](../../../../../../phenotype.md) [likelihood](../../../../../../likelihood-function.md) is therefore $27c/128$. It is the same at $\theta=0$ and $\theta=1/2$, so it cancels and **the LOD remains unchanged in this phenotype-only, independent-carrier extension**. If the identity of the affected child is specified, the factor is $9c/128$, which also cancels. No such conclusion applies automatically if new [genetic marker](../../../../../../genetic-marker.md) data are supplied or the revised [pedigree founder](../../../../../../founder-in-a-pedigree.md) model couples this branch to the old [genetic marker](../../../../../../genetic-marker.md) evidence.

In general an enlarged data set changes the score by

$$
\Delta Z=\log_{10}\frac{P(\text{new data}\mid\text{old data},\theta=0)}{P(\text{new data}\mid\text{old data},\theta=1/2)},
$$

after choosing a coherent model with positive [likelihood](../../../../../../likelihood-function.md). The additional affected child alone does not justify assigning it the [autozygosity](../../../../../../autozygosity.md) evidence of an affected child of a cousin marriage.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
