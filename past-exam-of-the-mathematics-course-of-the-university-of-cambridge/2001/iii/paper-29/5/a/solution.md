<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $I,J$ denote the two ordered [alleles](../../../../../../allele.md) at the [genetic locus](../../../../../../genetic-locus.md). Under [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md) they are independent with [probabilities](../../../../../../probability.md) $\pi_i,\pi_j$. Write the multiplicative [penetrance](../../../../../../penetrance.md) as $\mathbb P(D\mid I=i,J=j)=k\psi_i\psi_j$, with parameters chosen so these are valid [probabilities](../../../../../../probability.md), and set $Z=\sum_u\pi_u\psi_u$. Then

$$
\mathbb P(D)=k\sum_{i,j}\pi_i\pi_j\psi_i\psi_j=kZ^2.
$$

The [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
\boxed{\mathbb P(I=i,J=j\mid D)
=\frac{k\pi_i\pi_j\psi_i\psi_j}{kZ^2}
=\pi_i^*\pi_j^*,\qquad \pi_i^*=\frac{\pi_i\psi_i}{Z}.}
$$

Thus [multiplicative penetrance preserves Hardy-Weinberg equilibrium](../../../../../../multiplicative-penetrance-preserves-hardy-weinberg-equilibrium.md): the affected subjects still have two independent [allele](../../../../../../allele.md) draws, with tilted [allele](../../../../../../allele.md) frequencies. The displayed product uses ordered [allele](../../../../../../allele.md) slots. For the usual unordered [genotypes](../../../../../../genotype.md), the corresponding [probabilities](../../../../../../probability.md) are

$$
\boxed{\mathbb P(i/i\mid D)=(\pi_i^*)^2,\qquad
\mathbb P(i/j\mid D)=2\pi_i^*\pi_j^*\quad(i\ne j).}
$$

The factor of two is required for heterozygotes and must not be dropped when translating the ordered notation into [genotype](../../../../../../genotype.md) counts.

For [genetic association](../../../../../../genetic-association.md) analysis, the case [genotype](../../../../../../genotype.md) [probabilities](../../../../../../probability.md) factor into [allele](../../../../../../allele.md) frequencies, so under this model an allelic comparison with representative population controls is appropriate; separate dominance departures are not required by the [penetrance](../../../../../../penetrance.md) model. The ratio of case [allele](../../../../../../allele.md) frequency to population [allele](../../../../../../allele.md) frequency is proportional to $\psi_i$, and relative risk multipliers satisfy $\psi_i/\psi_j=(\pi_i^*/\pi_i)/(\pi_j^*/\pi_j)$. Population controls are important to this exact statement. Among specifically unaffected controls,

$$
\mathbb P(I=i,J=j\mid D^c)=\frac{\pi_i\pi_j(1-k\psi_i\psi_j)}{1-kZ^2},
$$

which generally does not factor. For a rare disease it is close to the population [genotype](../../../../../../genotype.md) law, but no rare-disease assumption was needed for the case factorization itself. [Population stratification](../../../../../../population-stratification.md) and sampling dependence must also be addressed before using an ordinary allelic [chi-squared test](../../../../../../chi-squared-test.md).

## ↑ Ancestors (11)

1. [A](../a.md)
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
