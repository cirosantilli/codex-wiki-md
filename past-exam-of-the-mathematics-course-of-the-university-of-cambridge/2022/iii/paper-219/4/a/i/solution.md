<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Using [Bayes' theorem](../../../../../../../bayes-theorem.md) and the fact that the prior is proper,

$$
\mathbb E_{\theta\mid y}\widehat I
=\int\frac1{p(y\mid\theta)}
\frac{p(y\mid\theta)p(\theta)}Z\,d\theta
=\frac1Z\int p(\theta)\,d\theta
=\frac1Z.
$$

Thus $\widehat I$ is an [unbiased estimator](../../../../../../../unbiased-estimator.md) of $Z^{-1}$, and the [Harmonic mean estimator of Bayesian model evidence](../../../../../../../harmonic-mean-estimator-of-bayesian-model-evidence.md) is $\widehat Z=1/\widehat I$. The reciprocal is not itself generally unbiased, though it is consistent when the [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md) applies.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
