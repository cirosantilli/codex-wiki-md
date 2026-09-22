<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B$ be the $n\times m$ matrix of [factor loadings](../../../../../../factor-loading.md), so $r=a+Bf$. A zero-cost [portfolio](../../../../../../investment-portfolio.md) $v$ with $\mathbf1^Tv=0$ and $B^Tv=0$ again has constant [financial payoff](../../../../../../contingent-claim-payoff.md) $v^Ta$. Absence of [arbitrage](../../../../../../arbitrage.md) implies

$$
a\in\operatorname{col}[\mathbf1\ B],\qquad
a=\lambda_0\mathbf1+B\kappa.
$$

Taking [expectations](../../../../../../expected-value.md) gives

$$
\boxed{\mathbb Er_i=\lambda_0+\sum_{j=1}^m b_{ij}\lambda_j,\qquad
\lambda_j=\kappa_j+\mathbb Ef_j.}
$$

If $[\mathbf1\ B]$ has full column [rank](../../../../../../rank-one-quadratic-form.md), a unit-cost [portfolio](../../../../../../investment-portfolio.md) with zero exposure to all factors exists and earns the certain rate $\lambda_0$. For each $j$, choose a zero-cost [portfolio](../../../../../../investment-portfolio.md) with loading one on factor $j$ and zero on the others; its [expected return](../../../../../../expected-return.md) is $\lambda_j$. Hence these coefficients are the rewards per unit systematic exposure, or factor [risk premiums](../../../../../../risk-premium.md), with the [financial payoff](../../../../../../contingent-claim-payoff.md) measured per unit of the chosen factor normalization. A traded [risk-free asset](../../../../../../risk-free-asset.md) fixes $\lambda_0$ to its return. Changing the scale or basis of the factors changes the coordinates of the [risk premiums](../../../../../../risk-premium.md) but leaves asset prices unchanged. With deficient [rank](../../../../../../rank-one-quadratic-form.md), only the spanned factor directions are identified and the coefficients need not be unique.

## ↑ Ancestors (11)

1. [C](../c.md)
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
