<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat $G_i$ as the entire [phase-known genotype](../../../../../../phase-known-genotype.md) of individual $i$ at the [genetic loci](../../../../../../genetic-locus.md) being studied, and let $\overline F$ denote the nonfounders. Assume unrelated [pedigree founders](../../../../../../founder-in-a-pedigree.md) have independent [genotype](../../../../../../genotype.md) priors, each nonfounder's [genotype](../../../../../../genotype.md) depends only on its parents' [genotypes](../../../../../../genotype.md), and the observed [phenotypes](../../../../../../phenotype.md) are conditionally independent given the [genotypes](../../../../../../genotype.md). These are the standard assumptions behind the [pedigree likelihood](../../../../../../pedigree-likelihood.md); shared environmental effects or related [pedigree founders](../../../../../../founder-in-a-pedigree.md) would require additional factors.

The directed ancestry graph is acyclic, even when there is [inbreeding](../../../../../../inbreeding.md). Order individuals with parents preceding offspring and apply the [chain rule for probabilities](../../../../../../chain-rule-for-probabilities.md). The parental [conditional independence](../../../../../../conditional-independence.md) assumption gives

$$
P(G_1,\ldots,G_n)=\prod_{i\in F}P(G_i)\prod_{i\in\overline F}P(G_i\mid G_{m(i)},G_{f(i)}).
$$

Conditional [phenotype](../../../../../../phenotype.md) [independence](../../../../../../independent-random-variables.md) gives $P(X_1,\ldots,X_n\mid G_1,\ldots,G_n)=\prod_iP(X_i\mid G_i)$. Multiplying these two expressions and summing over every possible latent [genotype](../../../../../../genotype.md) configuration proves

$$
\boxed{P(X_1,\ldots,X_n)=\sum_{G_1}\cdots\sum_{G_n}
\prod_iP(X_i\mid G_i)\prod_{i\in F}P(G_i)
\prod_{i\in\overline F}P(G_i\mid G_{m(i)},G_{f(i)}).}
$$

This is the [law of total probability](../../../../../../law-of-total-probability.md), not a claim that relatives have independent unconditional [genotypes](../../../../../../genotype.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
