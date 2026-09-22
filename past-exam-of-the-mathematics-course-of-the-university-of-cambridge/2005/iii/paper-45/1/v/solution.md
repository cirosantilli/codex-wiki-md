<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Take the affected sib pairs from independent families with the same disease model. Conditional on their marker sharing states, multiply the [recessive affected-sib-pair likelihoods](../../../../../../recessive-affected-sib-pair-likelihood.md):

$$
\mathcal L(\theta)=L_0^{n_0}L_1^{n_1}L_2^{n_2}.
$$

Write $x=\sqrt{L_0}=\theta(1-\theta)$, so that $\sqrt{L_2}=1/2-x$ and $L_1=x(1/2-x)$. Consequently

$$
\boxed{\mathcal L(\theta)=x^{\,2n_0+n_1}\left(\frac12-x\right)^{2n_2+n_1},\qquad 0\le x\le\frac14.}
$$

For an unordered count sample there can also be a [multinomial likelihood](../../../../../../multinomial-likelihood.md) coefficient, and the Mendelian [probabilities](../../../../../../probability.md) of the observed marker sharing states supply further factors. All these factors are independent of $\theta$.

If [genetic-study ascertainment](../../../../../../genetic-study-ascertainment.md) explicitly conditions on both children being affected, the normalizing disease [probability](../../../../../../probability.md) is constant:

$$
P(\text{both affected})=\frac14L_0+\frac12L_1+\frac14L_2=\frac{(x+1/2-x)^2}{4}=\frac1{16}.
$$

Thus the conditional sharing [likelihood](../../../../../../likelihood-function.md) differs from the displayed [likelihood function](../../../../../../likelihood-function.md) only by factors independent of the [recombination fraction](../../../../../../recombination-fraction.md). Multiple pairs drawn from the same larger sibship would not, in general, justify treating these pair [likelihoods](../../../../../../likelihood-function.md) as independent.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
