<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

A [sufficient statistic](../../../../../sufficient-statistic.md) is a function of the sample whose conditional sample distribution, given that statistic, does not depend on the parameter. The [factorization criterion for sufficiency](../../../../../fisher-neyman-factorization-theorem.md) states, for a dominated family, that $T$ is sufficient exactly when the joint density has form $g_\theta(T(x))h(x)$, where $h$ is independent of $\theta$.

Let $m=X_{(1)}=\min_iX_i$ and $M=X_{(n)}=\max_iX_i$. The joint [uniform density](../../../../../continuous-uniform-distribution.md) is

$$
f_{a,b}(x_1,\ldots,x_n)=(b-a)^{-n}1_{\{a\leq m,\ M\leq b\}},
$$

so $\boxed{T=(m,M)}$ is sufficient for $(a,b)$ by the [factorization criterion for sufficiency](../../../../../fisher-neyman-factorization-theorem.md). The [uniform order statistics](../../../../../uniform-order-statistic.md) have expectations

$$
\mathbb Em=a+\frac{b-a}{n+1},\qquad
\mathbb EM=a+\frac{n(b-a)}{n+1}.
$$

For example, the standardized minimum has survival probability $(1-t)^n$ on $[0,1]$, whose integral is $1/(n+1)$; the maximum follows by reflection. Solving these expectation equations gives the [unbiased estimator](../../../../../unbiased-estimator.md)

$$
\boxed{\widehat a=\frac{nm-M}{n-1},\qquad
\widehat b=\frac{nM-m}{n-1},\qquad
\mathbb E(\widehat a,\widehat b)=(a,b).}
$$

The assumption $n\geq2$ makes the denominator positive.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
