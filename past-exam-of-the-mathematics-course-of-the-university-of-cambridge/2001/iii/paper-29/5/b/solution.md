<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Label each parent's two [allele](../../../../../../allele.md) copies by its realized transmission: let $(A,B)$ be the transmitted and untransmitted [alleles](../../../../../../allele.md) of the first parent and $(C,D')$ those of the second. Under [random mating](../../../../../../panmixia.md) and [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md), the four parental [allele](../../../../../../allele.md) draws are independent with population frequencies $\pi$. Random [Mendelian segregation](../../../../../../mendelian-segregation.md) merely swaps the two independent copies within each parent, so the transmitted/untransmitted labelled pair still has [probability](../../../../../../probability.md) $\pi_a\pi_b$; the second pair has [probability](../../../../../../probability.md) $\pi_c\pi_d$.

The child receives $A,C$. If $\mathcal D$ is its disease event, its [penetrance](../../../../../../penetrance.md) is $k\psi_A\psi_C$ and its overall disease [probability](../../../../../../probability.md) is $kZ^2$. Therefore

$$
\boxed{\begin{aligned}
&\mathbb P(A=a,B=b,C=c,D'=d\mid\mathcal D)\\
&\qquad=\frac{k\psi_a\psi_c\pi_a\pi_b\pi_c\pi_d}{kZ^2}
=\pi_a^*\pi_c^*\pi_b\pi_d.
\end{aligned}}
$$

This proves the [transmitted and untransmitted alleles under multiplicative penetrance](../../../../../../transmitted-and-untransmitted-alleles-under-multiplicative-penetrance.md) factorization. Under these assumptions, the transmitted pair $a/c$ has the affected-case distribution, while the complementary pair $b/d$ has the population distribution and is independent of the transmitted pair. It is the [family pseudo-control genotype](../../../../../../family-pseudo-control-genotype.md).

As in part (a), the formula records labelled transmissions. When observed [genotypes](../../../../../../genotype.md) are unordered, sum over every compatible parental-origin transmission. This includes multiplicities for overlapping parental [alleles](../../../../../../allele.md) or two heterozygous parents producing a heterozygous child; it avoids interpreting one product as the total [probability](../../../../../../probability.md) of all observationally identical configurations. The homogeneous random-mating model is also essential to the unconditional independence: mixing ancestry strata can correlate the case and pseudo-control through their shared family background.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
