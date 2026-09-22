<h1 id="19d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $n\geq2$, use the unbiased residual variance $s^2=\mathrm{RSS}/(n-1)=n\widehat\sigma^2/(n-1)$. Under the null hypothesis, $(\widehat\beta-\beta_0)\sqrt{S_{xx}}/\sigma$ is standard normal and independent of $\mathrm{RSS}/\sigma^2\sim\chi^2_{n-1}$. Hence

$$
\boxed{T=\frac{(\widehat\beta-\beta_0)\sqrt{S_{xx}}}{s}\sim t_{n-1}\quad\text{under }H_0.}
$$

For a chosen significance level $\alpha$, reject the null in favor of the two-sided alternative exactly when $|T|>t_{n-1,1-\alpha/2}$, the stated upper quantile of the [Student t-distribution](../../../../../../student-s-t-distribution.md). The exact two-sided p-value is $2P(t_{n-1}\geq|T_{\rm obs}|)$. This [hypothesis test](../../../../../../statistical-hypothesis-test.md) does not substitute the biased MLE for $s^2$ without correcting its factor and does not use a normal critical value when variance is unknown.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [19D](../../19d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
