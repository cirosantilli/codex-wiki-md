<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Group means are [independent random variables](../../../../../../independent-random-variables.md) with [normal distributions](../../../../../../normal-distribution.md)

$$
\overline Y_i\sim N(\mu+\alpha_i,\sigma^2/J).
$$

The resulting univariate [sampling distributions](../../../../../../sampling-distribution.md) are

$$
\boxed{\widehat\mu\sim N(\mu,\sigma^2/J),\qquad
\widehat\alpha_2\sim N(\alpha_2,2\sigma^2/J).}
$$

The same [variance](../../../../../../variance-split.md) calculation holds for every $i\geq2$, since the difference involves two independent group means. Therefore the [standard errors](../../../../../../standard-error.md) satisfy

$$
\frac{\operatorname{se}(\widehat\alpha_i)}{\operatorname{se}(\widehat\mu)}
=\frac{\sqrt{2}\sigma/\sqrt J}{\sigma/\sqrt J}=\boxed{\sqrt2}.
$$

Replacing $\sigma$ by a common estimated error [standard deviation](../../../../../../standard-deviation.md) preserves this ratio. Although the individual group means are independent, the contrasts $\widehat\alpha_i$ share the baseline mean and have [covariance](../../../../../../covariance.md) $\sigma^2/J$ for distinct $i\geq2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
