<h1 id="a1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Both candidate models fit one parameter, but their parameter symbols have different meanings. For the [exponential distribution](../../../../../exponential-distribution.md) in model B,

$$
\ell_B(\theta_B)=N\log\theta_B-\theta_B\sum_i x_i,\qquad
\widehat\theta_B=\frac{N}{\sum_i x_i}=\frac{10}{7}.
$$

Its second derivative is $-N/\theta_B^2<0$, so this is its [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md). The maximized [log-likelihoods](../../../../../log-likelihood.md), including their normalization terms, are

$$
\ell_A(\widehat\theta_A)=1.262960000,\qquad
\ell_B(\widehat\theta_B)=4\log(10/7)-4=-2.573300224.
$$

Use the [corrected Akaike information criterion](../../../../../corrected-akaike-information-criterion.md) because $N=4$ is small relative to the number $k=1$ of fitted parameters:

$$
\operatorname{AICc}=-2\ell(\widehat\theta)+2k+\frac{2k(k+1)}{N-k-1}.
$$

The correction is $2$ for each model, giving

$$
\boxed{\operatorname{AICc}_A=1.47408,\qquad \operatorname{AICc}_B=9.14660}.
$$

**Prefer model A**, whose [corrected Akaike information criterion](../../../../../corrected-akaike-information-criterion.md) is smaller by $7.67252$. The ordinary [Akaike information criterion](../../../../../akaike-information-criterion.md) also gives that ranking because the two models receive equal penalties. This compares the two proposed models; it does not establish that either is a correct description of the process. The usual [corrected Akaike information criterion](../../../../../corrected-akaike-information-criterion.md) formula is a small-sample model-selection convention, rather than an exact finite-sample guarantee for these density families.

## ↑ Ancestors (13)

1. [H](../h.md)
2. [A1](../../a1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
