<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take “cousins” to [mean](../../../../../../expected-value.md) [first cousins](../../../../../../first-cousin.md) with unrelated, outbred founders and unrelated spouses in the intervening generation. Interpret a [homozygous](../../../../../../homozygosity.md) chromosome as two copies [identical by descent](../../../../../../identity-by-descent.md), and first use an idealization of independent, nonrecombining [chromosome](../../../../../../chromosome.md) blocks. Ordinary sequence [homozygosity](../../../../../../homozygosity.md) is a different quantity: unrelated copies can have the same allele, so its [probability](../../../../../../probability.md) also requires [allele frequencies](../../../../../../allele-frequency.md). Similarly, identity of an entire recombining chromosome requires a [genetic map](../../../../../../genetic-map.md), not just a pedigree.

At a single autosomal locus, the [probability](../../../../../../probability.md) of [autozygosity](../../../../../../autozygosity.md) in their child is the parents' [kinship coefficient](../../../../../../kinship-coefficient.md). Each of the two common grandparents contributes a path of length two from each parent, with [probability](../../../../../../probability.md) $(1/2)^{2+2+1}$. Thus the [first-cousin inbreeding coefficient](../../../../../../first-cousin-inbreeding-coefficient.md) is

$$
F=2(1/2)^5=1/16.
$$

If there are $L$ independent autosomal blocks, the [probability](../../../../../../probability.md) that none is autozygous is $(1-F)^L$. Hence the usual 23-block idealization gives

$$
\boxed{\Pr(\text{at least one autozygous block})=1-(15/16)^{23}.}
$$

The exponent describes the stated independent-block approximation; it is not a claim that all 23 human chromosome pairs inherit like autosomes.

Humans have 22 autosomal pairs. A son has one X and one Y and cannot have two homologous X copies. A daughter can have an autozygous X, with [probability](../../../../../../probability.md) $F_X$ determined by the [sex-linked cousin kinship](../../../../../../sex-linked-cousin-kinship.md) calculation in part (b). Thus a sex-aware version is

$$
\boxed{\Pr(\text{at least one autozygous paired block})=1-(15/16)^{22}(1-p_DF_X),}
$$

where $p_D$ is the [probability](../../../../../../probability.md) of a daughter, or is one or zero for a specified daughter's or son's sex. The [independent assortment](../../../../../../independent-assortment.md) approximation applies between the autosomes and the X. Opposite-sex parentage alone does not determine $F_X$: the parents may be cousins through their mothers, their fathers or one of each. Without these pedigree and chromosome-block assumptions, the wording does not specify a unique [probability](../../../../../../probability.md) of an entire homozygous human chromosome.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
