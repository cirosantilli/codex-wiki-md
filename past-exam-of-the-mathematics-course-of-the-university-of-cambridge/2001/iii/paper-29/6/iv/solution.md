<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $s$ index compatible parental phases in family 2, with fixed prior conditional weights $\pi_s$. For a given phase, let $r_s$ be the recombinant count and $m_s$ the informative-transmission count, absorbing any fixed [genotype](../../../../../../genotype.md) factors into $C_s$. The appropriate [pedigree likelihood](../../../../../../pedigree-likelihood.md) is

$$
\boxed{L_2(\theta)=\sum_s\pi_s C_s\theta^{r_s}(1-\theta)^{m_s-r_s}.}
$$

This is [phase averaging in a linkage likelihood](../../../../../../phase-averaging-in-a-linkage-likelihood.md); maximizing over a phase after observing the offspring would not be the same [likelihood](../../../../../../likelihood-function.md). In the common special case of two equally likely phases that exchange recombinant and nonrecombinant labels across $m_2$ transmissions, it reduces, up to a constant, to

$$
\tfrac12\{\theta^r(1-\theta)^{m_2-r}+\theta^{m_2-r}(1-\theta)^r\}.
$$

The constrained [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) compares all stationary points and endpoints on $[0,1/2]$.

**The actual phase set, weights, counts and numerical maximum for family 2 cannot be determined without its missing pedigree.** The special two-phase expression is a conditional example, not an assertion about this unidentified family.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
