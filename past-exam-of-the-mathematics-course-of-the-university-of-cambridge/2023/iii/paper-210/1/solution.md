<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F$, its [quantile function](../../../../../quantile-function.md) is the generalized inverse

$$
F^{-1}(u)=\inf\{x\in\mathbb R:F(x)\geq u\},
\qquad 0<u\leq1,
$$

with the infimum allowed to be $+\infty$. For observations $X_1,\ldots,X_n$, the [empirical distribution function](../../../../../empirical-distribution-function.md) is

$$
F_n(x)=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i\leq x\}}.
$$

If $X_{(1)}\leq\cdots\leq X_{(n)}$ are the [order statistics](../../../../../order-statistic.md), then

$$
X_{(j)}=F_n^{-1}(j/n).
$$

The [Bennett inequality](../../../../../bennett-inequality.md) says that if $Y_1,\ldots,Y_N$ are independent, $\mathbb EY_i=0$, $Y_i\leq b$ almost surely, and $\sum_i\mathbb EY_i^2\leq v$, then

$$
\mathbb P\left(\sum_iY_i\geq t\right)
\leq\exp\left[-\frac v{b^2}
h\left(\frac{bt}{v}\right)\right],
\qquad
h(u)=(1+u)\log(1+u)-u.
$$

To prove it, convexity of $e^{\lambda y}$ on $y\leq b$, followed by the power-series bound for centered $Y_i$, gives

$$
\mathbb Ee^{\lambda Y_i}
\leq\exp\left\{\frac{\mathbb EY_i^2}{b^2}
(e^{\lambda b}-1-\lambda b)\right\}.
$$

Independence and the [Chernoff bound](../../../../../chernoff-bound.md) therefore yield

$$
\mathbb P\left(\sum_iY_i\geq t\right)
\leq\exp\left\{-\lambda t+\frac v{b^2}
(e^{\lambda b}-1-\lambda b)\right\}.
$$

The minimizing value satisfies $e^{\lambda b}=1+bt/v$, namely $\lambda=b^{-1}\log(1+bt/v)$. Substitution gives the stated exponent.

For independent $U_i\sim\operatorname{Unif}[0,1]$, the [uniform order statistic](../../../../../uniform-order-statistic.md) satisfies

$$
U_{(j)}\sim\operatorname{Beta}(j,n-j+1),
\qquad
\mathbb EU_{(j)}=\frac j{n+1}.
$$

Set $p=j/(n+1)-x$. The event $U_{(j)}\leq p$ means that at least $j$ sample points lie in $[0,p]$. If this occurs, some $j$-element subset consists entirely of such points. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P(U_{(j)}\leq p)
\leq\binom njp^j
\leq\left(\frac{enp}{j}\right)^j.
$$

This is exactly the required inequality for $0\leq x<j/(n+1)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
