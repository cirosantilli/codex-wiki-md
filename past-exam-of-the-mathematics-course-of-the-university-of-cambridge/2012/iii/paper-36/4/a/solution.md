<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $e=y-g_\theta(x)$ and $h_\theta(x)=\partial g_\theta(x)/\partial\theta$. Holding the [nuisance parameter](../../../../../../nuisance-parameter.md) $\eta$ fixed, the parametric [score function](../../../../../../informant-function.md) is the [derivative](../../../../../../derivative.md) with respect to $\theta$ of the one-observation [log-likelihood](../../../../../../log-likelihood.md). The joint [probability density function](../../../../../../probability-density-function.md) is

$$
p_{\theta,\eta}(x,y)=\eta(x)\frac1{\sqrt{2\pi\sigma^2}}\exp\left(-\frac{(y-g_\theta(x))^2}{2\sigma^2}\right).
$$

Because $\partial e/\partial\theta=-h_\theta(x)$, differentiating gives

$$
\boxed{\dot\ell_{\theta,\eta}(x,y)=\frac{h_\theta(x)(y-g_\theta(x))}{\sigma^2}=\frac{h_\theta(x)e}{\sigma^2}.}
$$

For instance $E_\eta h_\theta(X)^2<\infty$ ensures a [square-integrable](../../../../../../square-integrable-function.md) [score function](../../../../../../informant-function.md). Its [expected value](../../../../../../expected-value.md) is zero by [independence](../../../../../../independent-random-variables.md) and the centered [normal distribution](../../../../../../normal-distribution.md) of the error. This is the [Gaussian regression score](../../../../../../gaussian-regression-score.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
