<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The selected zero-mean [autoregressive moving-average process](../../../../../../autoregressive-moving-average-model.md) is

$$
X_t=\phi X_{t-1}+\varepsilon_t+\theta\varepsilon_{t-1},
\qquad
\varepsilon_t\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The reported [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) are

$$
\widehat\phi=0.6997,
\qquad \widehat\theta=0.9510,
\qquad \widehat\sigma^2=0.4944.
$$

Using the displayed asymptotic standard error gives the [Wald confidence interval](../../../../../../wald-confidence-interval.md)

$$
0.9510\pm1.96(0.3287)=[0.307,1.595].
$$

This normal interval is unreliable and likely too narrow because the series has only about twenty observations, the moving-average estimate is near the noninvertibility boundary $\theta=1$, and the same data were used to select the model. The finite-sample likelihood is consequently skewed and model-selection uncertainty is omitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
