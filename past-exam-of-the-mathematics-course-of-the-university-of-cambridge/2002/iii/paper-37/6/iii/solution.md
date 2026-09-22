<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the usual genetic model in which disease outcomes are conditionally independent given the two individuals' [genotypes](../../../../../../genotype.md), and unshared founder [alleles](../../../../../../allele.md) are independently drawn from the same outbred population. Let $J$ denote their number of allele copies shared by [identity by descent](../../../../../../identity-by-descent.md). Conditional independence then gives

$$
\mathbb E(Y_1Y_2\mid G_1,G_2)=q_{G_1}q_{G_2}.
$$

When $J=2$, both individuals have the same genotype $G$. Its distribution remains the population genotype distribution under [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md), so their individual trait means are $K=p\alpha^2$ and

$$
\mathbb E(Y_1Y_2\mid J=2)=\mathbb E(q_G^2)=p^2\beta^2.
$$

Therefore

$$
\boxed{\operatorname{Cov}(Y_1,Y_2\mid J=2)
=p^2(\beta^2-\alpha^4)=V_G.}
$$

When $J=0$, all four unshared copies are independent, making $G_1,G_2$ independent population genotypes. Thus $\mathbb E(q_{G_1}q_{G_2})=(p\alpha^2)^2$ and

$$
\boxed{\operatorname{Cov}(Y_1,Y_2\mid J=0)=0.}
$$

**The residual-independence assumption is necessary.** Marginal penetrances alone do not determine joint disease probabilities. For example, with $\theta=1$, setting both traits equal to one shared [Bernoulli](../../../../../../bernoulli-distribution.md) variable of probability $p$ preserves every marginal penetrance, but gives covariance $p(1-p)$ even with no shared alleles. Shared environmental disease determinants or population structure therefore require an expanded model. The displayed answers are the intended locus-only covariance results, not a consequence of the penetrance table without that usual assumption.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
