<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume a single disease [allele](../../../../../../allele.md) $a$, complete [penetrance](../../../../../../penetrance.md) of $aa$, no disease in $Aa$ or $AA$, and [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) in the outbred population. If its population frequency is $q$, the disease prevalence is $q^2=10^{-6}$, so $q=10^{-3}$.

For a child with [inbreeding coefficient](../../../../../../inbreeding-coefficient.md) $F$, the two inherited copies are [identical by descent](../../../../../../identity-by-descent.md) with [probability](../../../../../../probability.md) $F$. In that component there is just one ancestral [allele](../../../../../../allele.md) draw, and it is $a$ with [probability](../../../../../../probability.md) $q$. In the remaining component there are two independent ancestral draws, with [probability](../../../../../../probability.md) $q^2$ of $aa$. Thus the [inbreeding genotype frequencies](../../../../../../inbreeding-genotype-frequencies.md) give

$$
P(aa)=Fq+(1-F)q^2=q^2+Fq(1-q).
$$

Using the [first-cousin inbreeding coefficient](../../../../../../first-cousin-inbreeding-coefficient.md) $F=1/16$, the disease-risk ratio is

$$
\boxed{\frac{P(aa)}{q^2}=1+\frac{F(1-q)}q=1+\frac{999}{16}=63.4375\simeq63.4.}
$$

The absolute risk in this model is $6.34375\times10^{-5}$. This calculation averages over the parental [genotypes](../../../../../../genotype.md) in first-cousin marriages before observing an affected child. It is not the risk conditional on both parents being known [genetic carriers](../../../../../../genetic-carrier.md), and assumes the specified cousin relationship is independent of disease status rather than conditioning on a selected disease [pedigree](../../../../../../pedigree.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
