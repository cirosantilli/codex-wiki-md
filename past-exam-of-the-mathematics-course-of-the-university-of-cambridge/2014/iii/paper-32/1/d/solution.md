<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $z=z_{1-\alpha}$. Under the [null hypothesis](../../../../../../null-hypothesis.md) rejection requires both $W_1\ge f$ and $W_2>z$. Since $W_2$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md),

$$
P_0(\text{reject})=\alpha-P_0(W_1<f,\ W_2>z).
$$

The [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) in the preceding calculation has a nonsingular [covariance matrix](../../../../../../covariance-matrix.md) and strictly positive [statistical probability density](../../../../../../probability-density-function.md) everywhere. For every finite [futility boundary](../../../../../../futility-boundary.md) $f$ and $0<\alpha<1$, the open rectangle $\{W_1<f,W_2>z\}$ has positive [probability](../../../../../../probability.md). Therefore

$$
\boxed{0<P_0(\text{reject})<\alpha.}
$$

For an explicit expression, conditional on $W_1=w$ the full-sample statistic is $N(w/\sqrt2,1/2)$ under the [null hypothesis](../../../../../../null-hypothesis.md), yielding

$$
P_0(\text{reject})=\int_f^\infty\phi(w)\left[1-\Phi(\sqrt2z-w)\right]dw.
$$

The [Type I error](../../../../../../type-i-and-type-ii-errors.md) is reduced because some otherwise rejecting paths stop for futility. Equality is approached as $f\to-\infty$, but does not hold at a finite [futility boundary](../../../../../../futility-boundary.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
