<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [empirical distribution function](../../../../../empirical-distribution-function.md) is $\widehat F_n(x)=n^{-1}\sum_i\mathbf1_{X_i\leq x}$. For continuous F, the [probability integral transform](../../../../../probability-integral-transform.md) gives independent uniform variables $U_i=F(X_i)$. Strict increase of F is unnecessary. More explicitly, generate the observations by $X_i=F^{-1}(U_i)$ with the generalized quantile inverse. Then $\mathbf1_{X_i\leq x}=\mathbf1_{U_i\leq F(x)}$, so $\widehat F_n(x)=G_n(F(x))$, where $G_n$ is the uniform empirical distribution.

Continuity and the limits of F ensure that its range contains $(0,1)$. The endpoint discrepancies for $G_n$ are zero. Hence

$$
\boxed{D_n\overset d=\sup_{0\leq u\leq1}|G_n(u)-u|,}
$$

which depends only on n. Equivalently it is $\max_{1\leq i\leq n}\{i/n-U_{(i)},U_{(i)}-(i-1)/n\}$, a function of uniform [order statistics](../../../../../order-statistic.md). This proves the distribution-free property of the [Kolmogorov-Smirnov statistic](../../../../../kolmogorov-smirnov-statistic.md) even when F has flat portions.

Choose $c_{n,\alpha}$ from this common distribution so that $\mathbb P(D_n\leq c_{n,\alpha})=1-\alpha$. The [Kolmogorov-Smirnov confidence band](../../../../../kolmogorov-smirnov-confidence-band.md) is

$$
\boxed{\max(0,\widehat F_n(x)-c_{n,\alpha})\leq F(x)\leq\min(1,\widehat F_n(x)+c_{n,\alpha})\quad\text{for all }x.}
$$

The event that all these inequalities hold is exactly the event used to choose the critical value, giving simultaneous coverage $1-\alpha$. The [Glivenko-Cantelli theorem](../../../../../glivenko-cantelli-theorem.md) states that for an independent identically distributed sample from any [distribution function](../../../../../cumulative-distribution-function.md), continuous or not, $\sup_x|\widehat F_n(x)-F(x)|\to0$ almost surely.

For an integrable r-argument [U-statistic kernel](../../../../../kernel-of-a-u-statistic.md), replace it by $h_s(x_1,\ldots,x_r)=(r!)^{-1}\sum_\pi h(x_{\pi(1)},\ldots,x_{\pi(r)})$. Every permutation has the same expectation by [exchangeability](../../../../../exchangeable-random-variables.md), so this [symmetrization of a U-statistic kernel](../../../../../symmetrization-of-a-u-statistic-kernel.md) preserves the target functional. For a symmetric [U-statistic kernel](../../../../../kernel-of-a-u-statistic.md) h and $n\geq r$, the [U-statistic](../../../../../u-statistic.md) is

$$
U_n={\binom nr}^{-1}\sum_{i_1<\cdots<i_r}h(X_{i_1},\ldots,X_{i_r}).
$$

Each summand has expectation theta, hence the statistic is unbiased.

For the population [variance](../../../../../variance-split.md), use $h(x,y)=(x-y)^2/2$. [Independence](../../../../../independent-random-variables.md) gives $\mathbb E(X_1-X_2)^2=2\operatorname{Var}(X_1)$ when the second moment is finite. The corresponding statistic simplifies using $\sum_{i<j}(X_i-X_j)^2=n\sum_i(X_i-\overline X)^2$:

$$
\boxed{U_n=\frac1{n(n-1)}\sum_{i<j}(X_i-X_j)^2=\frac1{n-1}\sum_i(X_i-\overline X)^2.}
$$

Thus [variance as a U-statistic](../../../../../variance-as-a-u-statistic.md) is precisely the usual unbiased [sample variance](../../../../../sample-variance.md), for $n\geq2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
