<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [empirical distribution function](../../../../../empirical-distribution-function.md) gives each observation mass $1/n$:

$$
\widehat F_n(x)=\frac1n\sum_{i=1}^n\mathbf1\{X_i\leq x\}.
$$

The [Glivenko-Cantelli theorem](../../../../../glivenko-cantelli-theorem.md) asserts the uniform, [almost sure convergence](../../../../../almost-sure-convergence.md)

$$
\boxed{\sup_{x\in\mathbb R}|\widehat F_n(x)-F(x)|\longrightarrow0\quad\text{almost surely}.}
$$

No [continuity](../../../../../continuous-function.md) of the [distribution function](../../../../../cumulative-distribution-function.md) is required. Here is a proof that also handles its jumps. Let $U_i$ be independent [uniform random variables](../../../../../uniform-random-variable.md) on $(0,1)$, and write $X_i=F^{-1}(U_i)$, where $F^{-1}(u)=\inf\{x:F(x)\geq u\}$. The generalized inverse property gives $\mathbf1\{X_i\leq x\}=\mathbf1\{U_i\leq F(x)\}$, so, if $G_n$ is the [empirical distribution function](../../../../../empirical-distribution-function.md) of the $U_i$, then $\widehat F_n(x)=G_n(F(x))$.

For a fixed [positive integer](../../../../../positive-integer.md) $m$, the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applied at each of the finitely many grid points $j/m$ shows that $\Delta_{n,m}=\max_{0\leq j\leq m}|G_n(j/m)-j/m|\to0$ [almost surely](../../../../../almost-sure-convergence.md). If $j/m\leq t\leq(j+1)/m$, [monotonicity](../../../../../monotonic-function.md) sandwiches $G_n(t)$ between its endpoint values, whence

$$
\sup_{0\leq t\leq1}|G_n(t)-t|\leq\Delta_{n,m}+\frac1m.
$$

Take the probability-one intersection of these events over all $m$. On that event the [limit superior](../../../../../limit-superior.md) is at most $1/m$ for every $m$, hence is zero. Therefore $\sup_x|G_n(F(x))-F(x)|\to0$. The coupled sequence has the same joint law as any independent sample from $F$, which proves the asserted almost sure conclusion for the original sample.

For $0<p<1$, the [sample quantile](../../../../../sample-quantile.md) is

$$
\widehat F_n^{-1}(p)=\inf\{x:\widehat F_n(x)\geq p\}=X_{(\lceil np\rceil)},
$$

where $X_{(j)}$ denotes the $j$th [order statistic](../../../../../order-statistic.md), with repeated observations retained. Suppose the population [median](../../../../../median.md) $m=F^{-1}(1/2)$ is unique and $F$ is [continuously differentiable](../../../../../continuously-differentiable-function.md) in a neighbourhood of $m$, with [probability density function](../../../../../probability-density-function.md) $f(m)>0$. Then

$$
\boxed{\sqrt n\bigl(\widehat F_n^{-1}(1/2)-m\bigr)\ \xrightarrow{d}\ N\!\left(0,\frac1{4f(m)^2}\right).}
$$

To see the [variance](../../../../../variance-split.md) directly, fix $t$ and count observations below $m+t/\sqrt n$. This count has a [binomial distribution](../../../../../binomial-distribution.md) with success probability $q_n=1/2+f(m)t/\sqrt n+o(n^{-1/2})$. The event that the [sample median](../../../../../sample-median.md) is below this point is that the count is at least $\lceil n/2\rceil$. The [central limit theorem](../../../../../central-limit-theorem.md) for this binomial triangular array gives a limiting probability $\Phi(2f(m)t)$, exactly the displayed [normal distribution](../../../../../normal-distribution.md). Centering is necessary for stating the limiting distribution; subtracting the deterministic population [median](../../../../../median.md) has no effect on the [asymptotic variance](../../../../../asymptotic-variance.md) requested in the comparisons.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
