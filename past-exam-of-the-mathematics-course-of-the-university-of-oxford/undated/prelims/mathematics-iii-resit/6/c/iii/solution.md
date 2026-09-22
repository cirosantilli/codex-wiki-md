<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [geometric distribution](../../../../../../../geometric-distribution.md) on positive integers, the [probability generating function](../../../../../../../probability-generating-function.md) is $p s/[1-(1-p)s]$. Conditional averaging over the red die yields

$$
\boxed{G_T(s)=\frac16\sum_{r=1}^6\frac{(7-r)s}{6-(r-1)s}
=\frac16\sum_{k=1}^6\frac{ks}{6-(6-k)s}.}
$$

As a [power series](../../../../../../../power-series.md), its exact domain of absolute convergence is

$$
\boxed{|s|<\frac65.}
$$

Indeed the slowest decaying component has failure [probability](../../../../../../../probability.md) $5/6$, so $\mathbb P(T=t)\ge(1/36)(5/6)^{t-1}$. At $|s|=6/5$, the terms of the [power series](../../../../../../../power-series.md) fail to tend to zero; outside that disk they grow. All six component series converge inside it. In particular, the [probability generating function](../../../../../../../probability-generating-function.md) is defined on the usual real [interval](../../../../../../../interval-mathematics.md) $0\le s\le1$, with $G_T(1)=1$. The rational expression beyond the convergence disk is only an algebraic continuation, not the defining [expected value](../../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
