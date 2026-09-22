<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [disease-ascertained transmission probability](../../../../../../disease-ascertained-transmission-probability.md) follows directly from [Bayes' theorem](../../../../../../bayes-theorem.md). Assume that, given the child's genotype $g$, its disease probability is a common baseline [penetrance](../../../../../../penetrance.md) times the [genotype relative risk](../../../../../../genotype-relative-risk.md) $R_g$, with no additional dependence on the parental genotypes. Write $q_g=P(g\mid g_f,g_m)$ for the [Mendelian segregation](../../../../../../mendelian-segregation.md) probability. Then

$$
\boxed{P(g\mid g_f,g_m,D)=\frac{q_gR_g}{\sum_hq_hR_h}.}
$$

There are four equally likely labelled parental transmission outcomes. For one specified outcome $t$, this becomes $P(t\mid g_f,g_m,D)=R_{g(t)}/\sum_{t'}R_{g(t')}$, which is the four-outcome interpretation of the displayed formula.

For an unordered child [genotype](../../../../../../genotype.md), let $m_g$ be the number of those outcomes producing it. Its probability is instead

$$
\boxed{P(g\mid g_f,g_m,D)=\frac{m_gR_g}{\sum_hm_hR_h}.}
$$

For example, two heterozygous parents have multiplicities $(1,2,1)$ for $11,12,22$. A heterozygous child therefore has probability $2R_{12}/(R_{11}+2R_{12}+R_{22})$. The four possible outcomes must be counted with multiplicity; treating their unordered genotypes as four distinct equally likely values would be incorrect.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
