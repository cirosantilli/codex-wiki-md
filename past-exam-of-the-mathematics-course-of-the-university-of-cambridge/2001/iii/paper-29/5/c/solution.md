<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The usual [transmission disequilibrium test](../../../../../../transmission-disequilibrium-test.md) conditions on the observed parental [genotypes](../../../../../../genotype.md), rather than modelling their population [probabilities](../../../../../../probability.md). For a heterozygous parent carrying $i,j$, the two transmission outcomes are equally likely under no association. With multiplicative [penetrance](../../../../../../penetrance.md), ascertainment through an affected child weights them by $\psi_i,\psi_j$, so

$$
\mathbb P(\text{transmit }i\mid\text{parent }i/j,\text{affected child})=\frac{\psi_i}{\psi_i+\psi_j}.
$$

The other parent's [penetrance](../../../../../../penetrance.md) factor cancels. This is a special case of [disease-ascertained transmission probability](../../../../../../disease-ascertained-transmission-probability.md). Under the null $\psi_i=\psi_j$, the [conditional probability](../../../../../../conditional-probability.md) is $1/2$. Count the discordant transmitted/untransmitted pairs from heterozygous parents and test their balance, using [McNemar's test](../../../../../../mcnemar-s-test.md) or its exact conditional binomial form. Homozygous parental transmissions do not distinguish the alternatives.

This conditional analysis removes the nuisance population [allele](../../../../../../allele.md) frequencies and retains the family matching. It is therefore robust to [population stratification](../../../../../../population-stratification.md), which can otherwise make [allele](../../../../../../allele.md) frequencies differ between cases and controls without a within-family transmission effect. It does not require the unconditional [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) and random-mating assumptions used for the population pseudo-control factorization. Independence of suitably sampled families, valid [genotypes](../../../../../../genotype.md) and the Mendelian null transmission model still matter.

**Prefer the within-family conditional transmission test to an unconditional population case–control analysis when the population-frequency assumptions and ancestry comparability are not secure.**

## ↑ Ancestors (11)

1. [C](../c.md)
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
