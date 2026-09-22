<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An exact finite [mixture model](../../../../../../mixture-model.md) follows from the [binomial theorem](../../../../../../binomial-theorem.md):

$$
(2+\theta)^{y_1}\theta^a(1-\theta)^b
=\sum_{z=0}^{y_1}\binom{y_1}{z}2^{y_1-z}\theta^{a+z}(1-\theta)^b,
\qquad a=y_4,\quad b=y_2+y_3.
$$

Define positive [mixture weights](../../../../../../mixture-weight.md)

$$
w_z=\frac{\binom{y_1}{z}2^{y_1-z}B(a+z+1,b+1)}{
\sum_{j=0}^{y_1}\binom{y_1}{j}2^{y_1-j}B(a+j+1,b+1)}.
$$

Here $B$ is the [Beta function](../../../../../../beta-function.md), so the component [probability distributions](../../../../../../probability-distribution.md) are $\operatorname{Beta}(a+z+1,b+1)$. All coefficients are computable from the observed integer counts.

Use [inverse transform sampling](../../../../../../inverse-transform-sampling.md) with the supplied $U$ to choose $Z$: writing $C_{-1}=0$ and $C_z=\sum_{j=0}^zw_j$, take $C_{Z-1}\leq U<C_Z$. Then recycle its position inside that interval,

$$
V=\frac{U-C_{Z-1}}{w_Z}.
$$

[Recycling a uniform random variable after discrete sampling](../../../../../../recycling-a-uniform-random-variable-after-discrete-sampling.md) makes $V$ uniform independently of $Z$, since $\Pr(Z=z,V\leq v)=w_zv$. It is also independent of all supplied [random variables](../../../../../../random-variable-split.md) with [gamma distributions](../../../../../../gamma-distribution.md). Transform these by the [probability integral transform](../../../../../../probability-integral-transform.md):

$$
W_i=1-e^{-G_i},\qquad 1\leq i\leq N.
$$

They are independent [random variables](../../../../../../random-variable-split.md) with [uniform distributions](../../../../../../continuous-uniform-distribution.md) because $G_i$ has a unit-rate [exponential distribution](../../../../../../exponential-distribution.md).

Conditional on $Z=z$, put $k=a+z+b+1$ and $r=a+z+1$. Form the $k$ values $V,W_1,\ldots,W_{k-1}$ and return their $r$th [order statistic](../../../../../../order-statistic.md). This uses at most the supplied $N$ [random variables](../../../../../../random-variable-split.md) with [gamma distributions](../../../../../../gamma-distribution.md), since $k-1=a+b+z\leq N$. The [uniform order statistic](../../../../../../uniform-order-statistic.md) formula gives

$$
\boxed{\Theta=\operatorname{order}_r(V,W_1,\ldots,W_{k-1}),\qquad
\Theta\mid Z=z\sim\operatorname{Beta}(a+z+1,b+1).}
$$

Averaging these component [probability density functions](../../../../../../probability-density-function.md) with weights $w_z$ recovers exactly the normalized [posterior density](../../../../../../posterior-density.md). Unused inputs can be discarded. When $N=0$, $Z=0$, $k=r=1$, and the output is $U$, as required. Interval endpoints and ties have [probability](../../../../../../probability.md) zero; any consistent convention there is harmless. Exactness here concerns the mathematical algorithm; finite-precision arithmetic can be stabilized with logarithmic [mixture weights](../../../../../../mixture-weight.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
