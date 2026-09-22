<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The baseline assay is a noisy measurement just like the follow-up assays. On the log scale, a [normal distribution](../../../../../../normal-distribution.md) for its error is a reasonable approximation if variability is approximately multiplicative on the original titre scale. The latent $\mu_{0i}$ represents the true baseline log-titre, with

$$
\boxed{y_{0i}\mid\mu_{0i},\sigma^2\sim N(\mu_{0i},\sigma^2).}
$$

Using a common [variance](../../../../../../variance-split.md) is a simplifying assumption justified if baseline and follow-up measurements have comparable assay variability; it should not be treated as a fact guaranteed by the study design. Treating $y_{0i}$ as exact ignores [measurement error](../../../../../../measurement-error.md) in a predictor and can lead to [attenuation bias from classical measurement error](../../../../../../attenuation-bias-from-classical-measurement-error.md) and understated uncertainty.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
