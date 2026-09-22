<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By the [invariance property of maximum likelihood estimation](../../../../../../invariance-property-of-maximum-likelihood-estimation.md),

$$
\boxed{\widehat h=10^{\widehat\theta/5}=e^{\widehat\theta/\alpha}.}
$$

The [sampling distribution](../../../../../../sampling-distribution.md) is $\widehat\theta\sim N(\theta,\sigma_{\widehat\theta}^2)$, where

$$
\sigma_{\widehat\theta}^2=C/K+H/N,
$$

$\widehat h$ has a [log-normal distribution](../../../../../../log-normal-distribution.md) with

$$
\log\widehat h\sim N\!\left(\log h,
\frac{\sigma_{\widehat\theta}^2}{\alpha^2}\right).
$$

Writing $v=\sigma_{\widehat\theta}^2/\alpha^2$, its exact fractional bias and variance are

$$
\frac{\mathbb E\widehat h-h}{h}=e^{v/2}-1,
\qquad
\frac{\operatorname{Var}(\widehat h)}{h^2}=e^v(e^v-1).
$$

Hence, to leading order,

$$
\boxed{\frac{\mathbb E\widehat h-h}{h}\simeq
\frac{\sigma_{\widehat\theta}^2}{2\alpha^2},
\qquad
\frac{\operatorname{Var}(\widehat h)}{h^2}\simeq
\frac{\sigma_{\widehat\theta}^2}{\alpha^2}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
