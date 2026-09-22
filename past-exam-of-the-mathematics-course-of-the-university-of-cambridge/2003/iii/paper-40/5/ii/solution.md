<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Distinguish the disease [alleles](../../../../../../allele.md) $D$ (normal) and $d$ (recessive disease) from the marker [alleles](../../../../../../allele.md) $A,a$. The affected mother and two affected children are $dd$. The unaffected father must be $Dd$, since he has affected children; the unaffected child is $Dd$, since the mother always transmits $d$. The mother is $AA$ at the marker, so the marker [genotypes](../../../../../../genotype.md) identify the father's transmissions to the three children as $a,A,A$. Their disease transmissions from the father are $d,d,D$.

The father's unphased double [heterozygosity](../../../../../../heterozygosity.md) has two possible pairs of [haplotypes](../../../../../../haplotype.md):

$$
s_1:AD/ad,\qquad s_2:Ad/aD.
$$

Under $s_1$, the three paternal transmissions $(ad,Ad,AD)$ are respectively nonrecombinant, recombinant and nonrecombinant. Under $s_2$, they are recombinant, nonrecombinant and recombinant. Each particular gamete has [probability](../../../../../../probability.md) $(1-\theta)/2$ or $\theta/2$, giving the conditional [pedigree likelihoods](../../../../../../pedigree-likelihood.md)

$$
L_1(\theta)=\frac{\theta(1-\theta)^2}{8},\qquad L_2(\theta)=\frac{\theta^2(1-\theta)}8.
$$

Assuming linkage equilibrium among founder [haplotypes](../../../../../../haplotype.md), the two phases have equal prior weights conditional on the observed paternal [genotype](../../../../../../genotype.md). [Phase averaging in a linkage likelihood](../../../../../../phase-averaging-in-a-linkage-likelihood.md) therefore gives

$$
\boxed{L(\theta)=\tfrac12L_1(\theta)+\tfrac12L_2(\theta)=\frac{\theta(1-\theta)}{16},\qquad0\le\theta\le\tfrac12.}
$$

Any factors for the parental [genotypes](../../../../../../genotype.md) omitted by this conditioning are constant in $\theta$. The derivative is $(1-2\theta)/16$, so **the maximum likelihood estimate is $\widehat\theta=1/2$ and there is no evidence for linkage**: the maximum [LOD score](../../../../../../lod-score.md) is zero. Choosing the best phase after observing the offspring would give a different and inappropriate calculation; the unknown phase must be averaged. The linkage-equilibrium assumption is modified explicitly in part (v).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
