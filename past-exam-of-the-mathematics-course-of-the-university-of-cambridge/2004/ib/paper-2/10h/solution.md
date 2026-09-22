<h1 id="10h/solution">Solution</h1>

↑ **Parent:** [10H](../10h.md)

For the first sampling design, treat the fixed groups of 60 and 90 people as two independent, representative samples from the respective populations. Within each sample, assume independent individuals with common eye-colour probabilities and mutually exclusive, exhaustive categories. This gives two independent [multinomial distributions](../../../../../multinomial-distribution.md). The [null hypothesis](../../../../../null-hypothesis.md) is that the two populations have the same eye-colour probabilities; its estimated common probabilities are $40/150$, $70/150$ and $40/150$.

The expected counts under the [null hypothesis](../../../../../null-hypothesis.md) are

$$
E=\begin{pmatrix}16&28&16\\24&42&24\end{pmatrix}.
$$

The [Pearson chi-squared test of homogeneity](../../../../../pearson-chi-squared-test-of-homogeneity.md) uses

$$
T=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}
=2\frac{16}{16}+\frac{64}{28}+2\frac{16}{24}+\frac{64}{42}
=\frac{50}{7}\simeq7.143.
$$

There are $2(3-1)=4$ unrestricted category parameters and $3-1=2$ under the [null hypothesis](../../../../../null-hypothesis.md), so the asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) has two [degrees of freedom](../../../../../degree-of-freedom.md). All expected counts exceed five, making the usual large-sample approximation reasonable. **Reject equality at the 5% level, but not at the 1% level**: $5.99<T<9.21$. The approximate [p-value](../../../../../p-value.md) is $\mathbb P(\chi_2^2\geq T)=e^{-25/7}\simeq0.0281$. Independence and representative sampling, rather than merely the count sizes, are essential to population inference; the result does not establish a causal explanation.

In the second design, the total sample size is fixed but both row and column classifications are observed for each sampled person. Assume an independent, representative sample with a common joint distribution of handedness and eye colour. The six cell counts then have one [multinomial distribution](../../../../../multinomial-distribution.md). The [null hypothesis](../../../../../null-hypothesis.md) is independence of the two classifications, so joint probabilities factor into row and column probabilities. Their [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) are the observed marginal proportions, again giving exactly $E$ above.

The unrestricted joint distribution has five free parameters; independence leaves $(2-1)+(3-1)=3$. The [Pearson chi-squared test of independence](../../../../../pearson-chi-squared-test-of-independence.md) again has two [degrees of freedom](../../../../../degree-of-freedom.md), the same statistic, and the same significance conclusion. **The numerical analysis is unchanged, but the sampling model changes from two fixed-row samples to one joint sample.** If handedness groups had instead been deliberately sampled with fixed row sizes, the first, homogeneity formulation would apply to those groups too.

## ↑ Ancestors (10)

1. [10H](../10h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
