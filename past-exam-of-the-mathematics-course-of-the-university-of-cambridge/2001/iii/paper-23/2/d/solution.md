<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For weights summing to one, collect the exact [portfolio](../../../../../../investment-portfolio.md) return as

$$
r^{(n)}=a^{(n)}+\sum_{j=1}^m b_j^{(n)}f_j+e_n,\qquad
a^{(n)}=\sum_iw_i a_i,\quad b_j^{(n)}=\sum_iw_ib_{ij},\quad e_n=\sum_iw_i\epsilon_i.
$$

The desired approximation means that $e_n\to0$, for example in [mean-square convergence](../../../../../../convergence-in-l2.md). Centering the residuals gives $\mathbb Ee_n=0$, but its [variance](../../../../../../variance-split.md) is

$$
\operatorname{Var}(e_n)=\sum_{i,k}w_iw_k\operatorname{Cov}(\epsilon_i,\epsilon_k).
$$

This identifies an omission in the printed hypotheses: bounded individual [variances](../../../../../../variance-split.md) do not control the cross terms. Indeed, take $\epsilon_i=Z$ for every $i$, where $Z$ is a nondegenerate centered [random variable](../../../../../../random-variable-split.md) with $\operatorname{Var}Z<s^2$. Equal weights $1/n<W/n$ for any $W>1$ retain $e_n=Z$ at every $n$. **The claimed diversification conclusion does not follow from the printed assumptions alone.**

Under the usual extra assumption that the residuals are pairwise uncorrelated and the weights are nonnegative, the advertised calculation is

$$
\mathbb Ee_n^2=\sum_iw_i^2\sigma_i^2
\le s^2\left(\max_iw_i\right)\sum_iw_i
\le\frac{s^2W}{n}\longrightarrow0.
$$

The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) then gives $\Pr(|e_n|>\delta)\le s^2W/(n\delta^2)\to0$. Alternatively, signed weights satisfying $|w_i|\le W/n$ give the bound $s^2W^2/n$. These are instances of the [covariance criterion for diversification of factor residuals](../../../../../../covariance-criterion-for-diversification-of-factor-residuals.md). More generally, with that absolute weight bound, $\sum_{i,k}|\operatorname{Cov}(\epsilon_i,\epsilon_k)|=o(n^2)$ suffices.

If [short selling](../../../../../../short-finance.md) are allowed, the printed one-sided weight bound is another insufficiency. Choose $0<c<W-1$, put $w_1=-c$ and $w_i=(1+c)/(n-1)$ for $i\ge2$, and let only $\epsilon_1$ be a nondegenerate centered residual. For all sufficiently large $n$ the one-sided bounds hold, but $e_n=-c\epsilon_1$ never vanishes. Thus nonnegative weights or an absolute bound is needed.

With the repaired assumptions, **well-diversified [portfolios](../../../../../../investment-portfolio.md) become approximately exposed only to the common factors**, and their residual [standard deviation](../../../../../../standard-deviation.md) is $O(n^{-1/2})$ in the uncorrelated case. The averaged coefficients may depend on $n$; convergence to fixed coefficients needs additional assumptions. In the associated asymptotic [arbitrage pricing theory](../../../../../../arbitrage-pricing-theory.md), diversifiable risk cannot command a persistent premium in well-diversified [portfolios](../../../../../../investment-portfolio.md) under absence of asymptotic [arbitrage](../../../../../../arbitrage.md), while common-factor exposure can. This does not prove an exact pricing equation for every individual noisy asset from the finite-market hypotheses alone.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
