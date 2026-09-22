<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With the usual variance-proxy convention for a [sub-Gaussian random vector](../../../../../../sub-gaussian-random-vector.md), every column inner product is a [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md) with proxy at most $\tau^2$. The two-sided [Chernoff bound](../../../../../../chernoff-bound.md) and [union bound](../../../../../../boole-s-inequality.md) imply

$$
\boxed{\|A^\top g\|_\infty\leq\tau\sqrt{2\log(2m/\delta)}\leq\sqrt2\tau\bigl(\sqrt{\log(2m)}+\sqrt{\log(1/\delta)}\bigr)}
$$

with [probability](../../../../../../probability.md) at least $1-\delta$. No [independence](../../../../../../independent-random-variables.md) between these inner products is required.

**The printed coefficient-one bound is false under this convention.** Take $k=m=1$, $A=[1]$, and $g=\pm\tau$ with equal [probability](../../../../../../probability.md). This [Rademacher random variable](../../../../../../rademacher-distribution.md) has the stipulated variance proxy, but for $\delta=0.99$ the printed threshold is less than $\tau$, whereas $|g|=\tau$ surely. Even a general sub-Gaussian assumption does not imply [Gaussian concentration inequality](../../../../../../gaussian-concentration-inequality.md) for arbitrary Lipschitz functions. Under the stronger convention $\mathbb E e^{\langle a,g\rangle}\leq e^{\tau^2\|a\|_2^2/4}$, the same [union bound](../../../../../../boole-s-inequality.md) proves the printed constants. That convention, however, differs from the binomial variance proxy used in 1(b).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
