<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $\alpha_1=0$, the marginal moment model gives

$$
\frac{\mathbb E(Y_{ij}\mid x_i)}{\mathbb E(Y_{i1}\mid x_i)}=e^{\alpha_j}.
$$

Thus **$e^{\alpha_2}$ and $e^{\alpha_3}$ are ratios of expected visits in Lent and Easter to expected visits in Michaelmas, respectively**, at the same baseline covariates. These are population mean ratios, including students with no propensity to attend; they are not [odds ratios](../../../../../../odds-ratio.md) or probabilities of any attendance.

In the hierarchical model, for a fixed positive student effect $b_i$, the conditional mean ratio is also $e^{\alpha_j}$. It describes a multiplicative within-student change in expected visits holding the student effect fixed. For the [structural-zero component](../../../../../../count-mixture-structural-zero.md) all three means are zero, so no nonzero ratio is defined there. Since the distribution of $b_i$ and the mixture weight do not vary by term, integrating out $b_i$ preserves this same marginal mean ratio. This is [mean-ratio preservation under a multiplicative random effect](../../../../../../mean-ratio-preservation-under-a-multiplicative-random-effect.md): the conditional and marginal term coefficients coincide for this multiplicative log-link model. They need not coincide in a general nonlinear mixed model, such as a logistic random-effect model. A log-mean difference $\alpha_j$ is not a difference of expected logarithms of counts, which can be undefined at zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
