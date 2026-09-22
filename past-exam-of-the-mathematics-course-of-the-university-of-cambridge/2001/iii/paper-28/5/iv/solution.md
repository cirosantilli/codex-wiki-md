<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A direct [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) can dichotomize satisfaction, for example high versus low-or-medium. In each covariate stratum use the high count as successes and the sum of the other counts as failures, with total $N_{ijk}$. This models $P(Y=\mathrm{high}\mid i,j,k)$ and is appropriate if that binary contrast is substantively intended, but discards distinctions among the merged categories. Another cutpoint gives a different binary question.

There is also an exact sequential binomial factorization preserving all three categories. With $p_1,p_2,p_3$ their probabilities in one stratum,

$$
n_1\sim\operatorname{Bin}(N,p_1),\qquad n_2\mid n_1\sim\operatorname{Bin}\left(N-n_1,\frac{p_2}{p_2+p_3}\right).
$$

Multiplying these two conditional [binomial likelihoods](../../../../../../binomial-likelihood.md) gives the [multinomial likelihood](../../../../../../multinomial-likelihood.md): the combinatorial coefficients multiply to $N!/(n_1!n_2!n_3!)$, and the probability factors reduce to $p_1^{n_1}p_2^{n_2}p_3^{n_3}$. [Continuation-ratio logits](../../../../../../continuation-ratio-logits.md) can therefore fit two logistic regressions, using the remaining stratum total as the second denominator. These are conditional stage models, not two independent counts with the same fixed denominator. Their regression restrictions need not equal those of the additive baseline-category model.

Finally, an ordinal analysis may fit cumulative binary contrasts and examine whether their slopes can be shared in a [proportional-odds model](../../../../../../proportional-odds-model.md). The binary indicators at different cutpoints from the same person are dependent. **Do not stack them as independent binomial observations and multiply their marginal likelihoods**; fit the joint ordinal likelihood or use a method with the appropriate dependence correction. This distinction separates a convenient descriptive collection of binary fits from a coherent multinomial or ordinal model.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
