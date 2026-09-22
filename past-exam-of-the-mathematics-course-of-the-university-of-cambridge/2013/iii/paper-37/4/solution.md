<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For any $s\geq0$, on the event $Y\geq0$ one has $e^{sY}\geq1$. The [Markov inequality](../../../../../markov-inequality.md) therefore gives $P(Y\geq0)\leq\mathbb E e^{sY}$, including the trivial value one at $s=0$. Taking the infimum proves the [Chernoff bound](../../../../../chernoff-bound.md).

For $s>0$ with finite [moment-generating functions](../../../../../moment-generating-function.md), [independence](../../../../../independent-random-variables.md) gives

$$
\log\mathbb E e^{sX}=s\sum_jn_j\alpha_j(s),\qquad
P(X\geq C)\leq\exp\left[s\left(\sum_jn_j\alpha_j(s)-C\right)\right].
$$

Consequently

$$
\boxed{\sum_jn_j\alpha_j(s)\leq C-\gamma/s\Longrightarrow P(X\geq C)\leq e^{-\gamma}}.
$$

An [effective bandwidth](../../../../../effective-bandwidth.md) is an exponential-moment measure of demand at a chosen tail parameter $s$: [independence](../../../../../independent-random-variables.md) makes these quantities additive. The spare capacity $\gamma/s$ pays for the desired exponential tail bound. For a cumulative-demand process over time $t$, the corresponding bandwidth would be $\log\mathbb E e^{sX(t)}/(st)$; here the time horizon is one. It is generally larger than mean demand because it charges for fluctuations, and [mathematical optimization](../../../../../mathematical-optimization-split.md) over $s$ selects the useful tradeoff.

For independent [normal distributions](../../../../../normal-distribution.md), put

$$
m=\sum_jn_j\lambda_j,\qquad v=\sum_jn_j\sigma_j^2.
$$

The [Gaussian effective bandwidth](../../../../../gaussian-effective-bandwidth.md) is $\alpha_j(s)=\lambda_j+s\sigma_j^2/2$. For $\gamma>0$ and $v>0$, the sufficient condition becomes $m+sv/2+\gamma/s\leq C$. Its left side is minimized at $s_*=(2\gamma/v)^{1/2}$, giving

$$
\boxed{m+\sqrt{2\gamma v}\leq C\Longrightarrow P(X\geq C)\leq e^{-\gamma}}.
$$

This is a sufficient Chernoff safety margin, not the exact normal tail quantile.

Indeed $X\sim N(m,v)$, so, writing $\Phi$ for the [standard normal distribution function](../../../../../standard-normal-distribution-function.md),

$$
P(X\geq C)=1-\Phi\left(\frac{C-m}{\sqrt v}\right).
$$

The [exact Gaussian chance constraint](../../../../../exact-gaussian-chance-constraint.md) is therefore

$$
\boxed{m+\phi\sqrt v\leq C,\qquad\phi=\Phi^{-1}(1-e^{-\gamma})}.
$$

This is necessary and sufficient when $v>0$, even when $\phi$ is negative. The Chernoff coefficient $\sqrt{2\gamma}$ is more conservative.

There is an important boundary qualification. If $v=0$, then $X=m$ deterministically, and for $\gamma>0$ the exact requirement is **$C>m$**, not $C\geq m$. For example, $X\equiv0$, $C=0$, $\gamma=1$ satisfies the printed square-root condition but has $P(X\geq C)=1>e^{-1}$. Thus both Gaussian non-strict displayed forms require positive total [variance](../../../../../variance-split.md), which follows if at least one flow is present and its [variance](../../../../../variance-split.md) is positive. With no positive [variance](../../../../../variance-split.md), the [deterministic boundary in an upper-tail chance constraint](../../../../../deterministic-boundary-in-an-upper-tail-chance-constraint.md) must be treated separately. If $\gamma\leq0$, the target upper bound is at least one and imposes no restriction; the displayed square-root discussion naturally assumes $\gamma>0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
