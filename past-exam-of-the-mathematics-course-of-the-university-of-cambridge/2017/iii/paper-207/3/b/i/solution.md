<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Condition on each patient's initial observed state and assume [independent](../../../../../../../independent-random-variables.md) patient trajectories and observation times that do not carry additional information about the unobserved path. The [Markov property](../../../../../../../markov-property.md) factors each trajectory's [likelihood function](../../../../../../../likelihood-function.md) into its successive one-year [transition probabilities](../../../../../../../transition-probability.md). Thus

$$
\boxed{\ell(\lambda,\mu)=\sum_{r,s=1}^2n_{rs}\log p_{rs}(1;\lambda,\mu).}
$$

More explicitly, with $q=\lambda+\mu>0$ and $E=e^{-q}$,

$$
\ell=n_{11}\log\frac{\mu+\lambda E}{q}+n_{12}\log\frac{\lambda(1-E)}q+n_{21}\log\frac{\mu(1-E)}q+n_{22}\log\frac{\lambda+\mu E}q.
$$

Successive transitions within one patient need not be [independent](../../../../../../../independent-random-variables.md) unconditionally: this is a product of conditional factors justified by the [Markov property](../../../../../../../markov-property.md). If initial-state [probabilities](../../../../../../../probability.md) are modeled rather than conditioned on, their [likelihood contributions](../../../../../../../likelihood-contribution.md) must also be included. Zero-count terms contribute zero; a positive count attached to a zero model [probability](../../../../../../../probability.md) makes the [log-likelihood](../../../../../../../log-likelihood.md) equal to $-\infty$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
