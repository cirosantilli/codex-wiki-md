<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume the parents are unaffected, the disease has complete [penetrance](../../../../../../penetrance.md) with a single recessive causal [allele](../../../../../../allele.md), and there are no phenocopies, new disease [mutations](../../../../../../mutation.md) or alternative causal loci. An affected first child has [genotype](../../../../../../genotype.md) $aa$, so each unaffected parent must be a [heterozygote](../../../../../../heterozygote.md) $Aa$. Conditional on these parental [genotypes](../../../../../../genotype.md), [Mendelian segregation](../../../../../../mendelian-segregation.md) in the second child's paternal and maternal [meioses](../../../../../../meiosis.md) is independent of the transmissions to the first child. Therefore

$$
\boxed{P(\text{second affected}\mid\text{first affected, parents unaffected})=\frac12\cdot\frac12=\frac14.}
$$

**This is the same sibling recurrence risk as for unrelated, unaffected parents under the same recessive model.** Parental kinship increases the [prior](../../../../../../prior-probability.md) [probability](../../../../../../probability.md) that both parents carry the same rare disease [allele](../../../../../../allele.md); after both are identified as carriers, it does not alter their Mendelian transmission [probabilities](../../../../../../probability.md). The factor $63.4$ from the preceding part is therefore not an additional multiplier on the [sibling recurrence risk](../../../../../../sibling-recurrence-risk.md).

If unaffected parents are not explicitly required, the rare-disease assumption is an approximation supporting the usual carrier-by-carrier calculation, rather than a logically exact consequence of an affected child alone. Under complete [penetrance](../../../../../../penetrance.md), the compatible parental matings are $Aa\times Aa$, $Aa\times aa$ and $aa\times aa$, with second-child risks $1/4,1/2,1$ respectively. Let their [prior](../../../../../../prior-probability.md) [probabilities](../../../../../../probability.md) be $w_{11},w_{12},w_{22}$, including both orders in $w_{12}$. Conditioning on the affected first child gives

$$
P(\text{second affected}\mid\text{first affected})=\frac{w_{11}/16+w_{12}/4+w_{22}}{w_{11}/4+w_{12}/2+w_{22}}.
$$

Without negligible or excluded affected-parent matings, this mixture need not equal $1/4$ and may depend on consanguinity. Likewise incomplete [penetrance](../../../../../../penetrance.md) or disease heterogeneity invalidates the assertion that an affected child of unaffected parents necessarily identifies an $Aa\times Aa$ mating. The stated $1/4$ answer uses the unaffected-parent, fully penetrant single-locus assumptions.

## ↑ Ancestors (11)

1. [D](../d.md)
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
