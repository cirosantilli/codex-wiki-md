<h1 id="8h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sample mean $\overline X$ has [normal distribution](../../../../../../normal-distribution.md) $N(\mu,1/n)$ because the observations are independent with known variance 1. The [pivotal quantity](../../../../../../pivotal-quantity.md) $Z=\sqrt n(\overline X-\mu)$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md). Consequently

$$
\mathbb P_\mu\left\{-1.96\le\sqrt n(\overline X-\mu)\le1.96\right\}\simeq0.95,
$$

and inversion gives the [confidence interval](../../../../../../confidence-interval.md)

$$
\boxed{\left[\overline X-\frac{1.96}{\sqrt n},\ \overline X+\frac{1.96}{\sqrt n}\right].}
$$

Replacing 1.96 by the exact $0.975$ normal quantile gives exact 95% coverage; the printed numerical value gives the usual rounded interval. No variance estimation or Student distribution is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8H](../../8h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
