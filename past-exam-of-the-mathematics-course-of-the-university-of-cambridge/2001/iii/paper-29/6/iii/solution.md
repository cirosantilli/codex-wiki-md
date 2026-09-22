<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For known parental [haplotypes](../../../../../../haplotype.md), count $r_1$ recombinant transmissions among $m_1$ informative meioses. The conditional [pedigree likelihood](../../../../../../pedigree-likelihood.md) has the form

$$
L_1(\theta)=C_1\theta^{r_1}(1-\theta)^{m_1-r_1},
$$

where $C_1$ contains parameter-independent gamete and [genotype](../../../../../../genotype.md) factors. Differentiating its logarithm gives $r_1/\theta-(m_1-r_1)/(1-\theta)$, so the constrained [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta_1=\min\{r_1/m_1,\tfrac12\}\quad(m_1>0).}
$$

When $r_1=0$ the maximum is at zero; if no meiosis is informative, the [likelihood](../../../../../../likelihood-function.md) is constant and the parameter is not estimable from that family. This formula presumes the family phase has been resolved; otherwise use [phase averaging in a linkage likelihood](../../../../../../phase-averaging-in-a-linkage-likelihood.md) first.

**The family-specific value cannot be calculated because its pedigree, phases and transmission counts are absent from the supplied PDF.** The missing data cannot be reconstructed from the requested estimate alone.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
