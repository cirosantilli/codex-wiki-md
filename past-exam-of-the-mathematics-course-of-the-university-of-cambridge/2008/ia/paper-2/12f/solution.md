<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Use the positive-support convention for the [geometric distribution](../../../../../geometric-distribution.md) and put $q=1-p$. Differentiating the convergent [geometric series](../../../../../geometric-series.md) $\sum_{k\geq0}q^k=(1-q)^{-1}$ gives

$$
\sum_{k\geq1}kq^{k-1}=\frac1{(1-q)^2},\qquad
\sum_{k\geq2}k(k-1)q^{k-2}=\frac2{(1-q)^3}.
$$

Consequently

$$
\mathbb EY=p\sum_{k\geq1}kq^{k-1}=\frac1p,\qquad
\mathbb E[Y(Y-1)]=pq\sum_{k\geq2}k(k-1)q^{k-2}=\frac{2q}{p^2}.
$$

Subtracting the square of the [expectation](../../../../../expected-value.md) from the [second moment](../../../../../second-moment.md) yields

$$
\boxed{\mathbb EY=\frac1p,\qquad\operatorname{Var}(Y)=\frac{1-p}{p^2}.}
$$

For the die, this is the [coupon collector problem](../../../../../coupon-collector-problem.md). When $r$ scores are still missing, let $W_r$ count rolls up to and including the next newly observed score. Every fresh roll has success [probability](../../../../../probability.md) $r/6$, so $W_r$ has a [geometric distribution](../../../../../geometric-distribution.md) of parameter $r/6$. These six successive waiting times are [independent](../../../../../independent-random-variables.md): conditional on the entire past at the start of a stage, its waiting-time distribution depends only on the number $r$, not on the identities of the missing scores. Iterated conditioning therefore factors their joint distribution. The total number of rolls is $N=\sum_{r=1}^6W_r$.

Using [linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\boxed{\mathbb EN=\sum_{r=1}^6\frac6r
=6\left(1+\frac12+\frac13+\frac14+\frac15+\frac16\right)
=\frac{147}{10}=14.7.}
$$

Using [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md), or the [coupon collector waiting-time variance](../../../../../coupon-collector-waiting-time-variance.md) formula just derived by this decomposition, gives

$$
\operatorname{Var}(N)=\sum_{r=1}^6\frac{1-r/6}{(r/6)^2}
=\sum_{r=1}^6\left[\left(\frac6r\right)^2-\frac6r\right]
=\frac{5369}{100}-\frac{147}{10}=\frac{3899}{100}.
$$

Hence the requested [standard deviation](../../../../../standard-deviation.md) is

$$
\boxed{\operatorname{sd}(N)=\frac{\sqrt{3899}}{10}\approx6.2442.}
$$

The hint rounds the sum of squares from $53.69$ to $53.7$; using that rounded value gives $\sqrt{39}\approx6.245$, consistent at the precision of the hint. The exact computation preserves the slightly more precise value above.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
