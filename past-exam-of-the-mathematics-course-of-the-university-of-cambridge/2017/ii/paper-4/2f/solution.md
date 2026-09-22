<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

For $x>0$, $N(x)=\lfloor1/x\rfloor$ and $T(x)=1/x-\lfloor1/x\rfloor$. Iterating this [Gauss continued-fraction map](../../../../../gauss-continued-fraction-map.md) on an [irrational number](../../../../../irrational-number.md) never reaches zero, and its [continued fraction](../../../../../continued-fraction.md) is

$$
\boxed{x=[0;N(x),N(Tx),N(T^2x),\ldots].}
$$

The branches $T:(1/(n+1),1/n)\to(0,1)$ have inverse $x_n(y)=1/(n+y)$, for $n\geq1$. The [change of variables formula](../../../../../change-of-variables-formula.md) for a [probability density function](../../../../../probability-density-function.md) gives, [almost everywhere](../../../../../almost-everywhere.md),

$$
f_{T(X)}(y)=\sum_{n=1}^\infty f\!\left(\frac1{n+y}\right)\frac1{(n+y)^2}
=\frac1{\log2}\sum_{n=1}^\infty\left[\frac1{n+y}-\frac1{n+y+1}\right]
=\frac1{(\log2)(1+y)}.
$$

The endpoints of these branches are a [countable set](../../../../../countable-set.md) of probability zero. Thus **$T(X)$ and $X$ have the same distribution**; this [Gauss measure](../../../../../gauss-measure.md) is an [invariant measure](../../../../../invariant-measure.md) for the [Gauss continued-fraction map](../../../../../gauss-continued-fraction-map.md).

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
