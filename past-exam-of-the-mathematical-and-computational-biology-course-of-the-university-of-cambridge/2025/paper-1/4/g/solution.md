<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [Poisson generalized linear mixed model](../../../../../poisson-generalized-linear-mixed-model.md) assumes conditionally [Poisson distributed](../../../../../poisson-distribution.md) counts with a [log link](../../../../../logarithmic-link-function.md). The fitted [variance components](../../../../../variance-component.md) are both zero, so this fit lies on a boundary and reduces to ordinary [Poisson regression](../../../../../poisson-regression.md). It estimates

$$
\widehat\mu(a)=\exp(0.793+0.064a),\qquad
\boxed{\frac{\widehat\mu(a+1)}{\widehat\mu(a)}=e^{0.064}\simeq1.066}.
$$

Thus the fitted annual increase is about **6.6%**, with approximate 95% [confidence interval](../../../../../confidence-interval.md) for the [rate ratio](../../../../../rate-ratio.md) $(e^{0.001},e^{0.128})\simeq(1.001,1.137)$. The age evidence is much weaker than in the Gaussian fit: the quoted [p-value](../../../../../p-value.md) is $0.047$. Zero estimated group variances do not prove that real bird and year differences are absent.

The [Poisson distribution](../../../../../poisson-distribution.md) forces conditional [variance](../../../../../variance-split.md) to equal the conditional [expected value](../../../../../expected-value-split.md). Here fitted means are around two to three hatchlings, whereas the Gaussian model estimated a residual [variance](../../../../../variance-split.md) of only $0.188$. This suggests checking [underdispersion](../../../../../underdispersion.md) and the bounded nature of hatching counts, rather than assuming a Poisson response solves the diagnostic problems. Inspect simulated count residuals and predictive distributions; if the number of eggs is observed, fit a binomial mixed model and check that model's dispersion too.

The displayed Gaussian and Poisson [Akaike information criterion](../../../../../akaike-information-criterion.md) values should not simply be ranked as if they used the same likelihood convention: one evaluates a continuous density and the other a probability mass. Compare properly specified count models on the same observed response scale, with compatible likelihoods and predictive checks. A boundary fit, doubtful dispersion assumptions, and possible nonlinear age effects all warrant further work before a strong biological conclusion.

## ↑ Ancestors (13)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
