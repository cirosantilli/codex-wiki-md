<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Using the same [Bayesian deviance](../../../../../../bayesian-deviance.md) convention, the [deviance information criterion](../../../../../../deviance-information-criterion.md) and [Akaike information criterion](../../../../../../akaike-information-criterion.md) are

$$
\boxed{\operatorname{DIC}=\overline D+p_D=D(\overline\theta)+2p_D,\qquad
\operatorname{AIC}=D(\widehat\theta)+2p.}
$$

Both combine a lack-of-fit term with a complexity penalty; smaller values are preferred among comparable models. Under the locally flat [prior distribution](../../../../../../prior-probability.md) and the regular [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) approximation, $D(\overline\theta)\approx D(\widehat\theta)$ and $p_D\approx p$, so

$$
\boxed{\operatorname{DIC}\approx D(\widehat\theta)+2p=\operatorname{AIC}.}
$$

All fitted parameters counted in the likelihood, including unknown dispersion parameters, belong in $p$. The equivalence need not hold for informative priors, nonregular models, or different choices of the likelihood's latent-variable representation.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
