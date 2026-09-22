<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Assume the known variances are positive and write $\bar x=n^{-1}\sum_ix_i$. The [likelihood](../../../../../likelihood-function.md) times the normal [prior distribution](../../../../../prior-probability.md) is proportional to

$$
\exp\left\{-\frac12\left[\frac1{\sigma^2}\sum_i(x_i-\theta)^2+
\frac{(\theta-\mu)^2}{\tau^2}\right]\right\}.
$$

Collecting the quadratic and linear terms in $\theta$ completes the square with precision $v^{-1}=n/\sigma^2+1/\tau^2$ and mean $m=v(n\bar x/\sigma^2+\mu/\tau^2)$. Thus [normal-normal conjugacy](../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives

$$
\boxed{\theta\mid x_1,\ldots,x_n\sim N(m,v),\qquad
v=\frac{\sigma^2\tau^2}{\sigma^2+n\tau^2},\quad
m=\frac{n\tau^2\bar x+\sigma^2\mu}{\sigma^2+n\tau^2}.}
$$

For [quadratic loss](../../../../../squared-error-loss.md), the posterior risk of reporting $a$ is $\mathbb E[(a-\theta)^2\mid x]=v+(a-m)^2$, uniquely minimized at $a=m$. For [absolute-error loss](../../../../../absolute-error-loss.md), differentiating the posterior risk gives $2F_{\theta\mid x}(a)-1$, so its minimizer is a posterior median. The normal posterior is symmetric about $m$ and has a strictly increasing distribution function, hence that median is uniquely $m$. Therefore **both optimal point estimates equal $m$**, the [posterior mean](../../../../../posterior-mean.md).

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
