<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $Q(u)=\inf\{x\in\mathbb R:F(x)\geq u\}$ for $0<u<1$. This is the [quantile function](../../../../../quantile-function.md), rather than an ordinary inverse requiring strict increase. The limits of the [distribution function](../../../../../cumulative-distribution-function.md) at infinity make $Q(u)$ finite, and the fact that $F$ is a [right-continuous function](../../../../../right-continuous-function.md) ensures $F(Q(u))\geq u$. Consequently

$$
Q(u)\leq x\quad\Longleftrightarrow\quad u\leq F(x).
$$

Increasing $u$ shrinks the set in the [infimum](../../../../../infimum.md), so the [quantile function](../../../../../quantile-function.md) is a [monotone function](../../../../../monotonic-function.md). To prove the [left continuity of the quantile function](../../../../../left-continuity-of-the-quantile-function.md), fix $u$ and let $L=\sup_{v<u}Q(v)\leq Q(u)$. If $L<Q(u)$, choose $L<y<Q(u)$. Then $F(y)<u$, so some $v\in(F(y),u)$ satisfies $Q(v)>y$, a contradiction. Thus **$Q(v)\uparrow Q(u)$ as $v\uparrow u$**. At a flat stretch of the [distribution function](../../../../../cumulative-distribution-function.md), the [quantile function](../../../../../quantile-function.md) may jump immediately to the right, consistent with this left-continuous convention.

For the [uniform order statistic](../../../../../uniform-order-statistic.md), count the observations at most $u$. That count has the [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,u$, giving

$$
\mathbb P\{U_{(j)}\leq u\}=\sum_{r=j}^n\binom nr u^r(1-u)^{n-r},\qquad 0<u<1.
$$

Differentiating makes adjacent terms telescope: use $r\binom nr=n\binom{n-1}{r-1}$ and $(n-r)\binom nr=n\binom{n-1}{r}$. The [probability density function](../../../../../probability-density-function.md) is therefore

$$
\boxed{g_j(u)=\frac{n!}{(j-1)!(n-j)!}u^{j-1}(1-u)^{n-j}\mathbf1_{\{0<u<1\}}.}
$$

In particular, $U_{(j)}$ has the [Beta distribution](../../../../../beta-distribution.md) with parameters $j,n-j+1$.

Write $m=Q(1/2)$ for the specified [median](../../../../../median.md). [Continuity](../../../../../continuous-function.md) of the [distribution function](../../../../../cumulative-distribution-function.md) gives $F(m)=1/2$ and no mass at $m$, even if the [distribution function](../../../../../cumulative-distribution-function.md) has a flat stretch there. Thus $B=\sum_i\mathbf1_{\{X_i<m\}}$ has the [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,1/2$. Except on a null event, the [order-statistic confidence interval for a median](../../../../../order-statistic-confidence-interval-for-a-median.md) covers $m$ exactly when $j\leq B\leq n-j$. Symmetry of the [binomial distribution](../../../../../binomial-distribution.md) makes its two failure probabilities equal. Alternatively, the [probability integral transform](../../../../../probability-integral-transform.md) gives

$$
\mathbb P\{B\geq n-j+1\}
=\mathbb P\{U_{(n-j+1)}\leq1/2\}
=n\binom{n-1}{j-1}\int_0^{1/2}u^{n-j}(1-u)^{j-1}\,du.
$$

Hence **the coverage is exactly $1-\alpha$**, with

$$
\boxed{\alpha=2n\binom{n-1}{j-1}\int_0^{1/2}u^{n-j}(1-u)^{j-1}\,du
=2\sum_{r=0}^{j-1}\binom nr2^{-n}.}
$$

The asymmetric open/closed endpoint convention does not change the coverage because the [continuous probability distribution](../../../../../continuous-probability-distribution-split.md) assigns no mass to the [median](../../../../../median.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
