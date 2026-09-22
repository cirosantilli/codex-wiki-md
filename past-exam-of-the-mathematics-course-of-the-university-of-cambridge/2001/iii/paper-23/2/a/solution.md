<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use unrestricted long and short [portfolios](../../../../../../investment-portfolio.md), as required by the usual [arbitrage pricing theory](../../../../../../arbitrage-pricing-theory.md) argument. A vector $v\in\mathbb R^n$ of initial monetary positions with $\mathbf1^Tv=0$ costs zero. Its terminal [financial payoff](../../../../../../contingent-claim-payoff.md), in the exact one-factor model, is

$$
v^T(\mathbf1+r)=v^Ta+(v^Tb)f.
$$

If also $v^Tb=0$, the [financial payoff](../../../../../../contingent-claim-payoff.md) is the constant $v^Ta$. A nonzero value would be an [arbitrage](../../../../../../arbitrage.md) after choosing the sign of $v$. Absence of [arbitrage](../../../../../../arbitrage.md) thus says that $a$ annihilates $\ker[\mathbf1\ b]^T$. By finite-dimensional [linear algebra](../../../../../../linear-algebra-split.md),

$$
a\in(\ker[\mathbf1\ b]^T)^\perp=\operatorname{span}\{\mathbf1,b\}.
$$

Write $a=\lambda_0\mathbf1+\kappa b$. Taking [expectations](../../../../../../expected-value.md), assuming the factor has finite mean, proves

$$
\boxed{\bar r_i=\lambda_0+b_i\lambda_1,\qquad\lambda_1=\kappa+\mathbb Ef.}
$$

This is [exact factor pricing without a traded risk-free asset](../../../../../../exact-factor-pricing-without-a-traded-risk-free-asset.md). The PDF prints an asset-indexed $\lambda_i$; the stronger valid result has the same $\lambda_1$ for every asset, so it also satisfies the printed relation by taking all its $\lambda_i$ equal. If every loading is equal, the spanning vectors are dependent and the coefficients need not be unique. For a nondegenerate factor and a zero-exposure unit-cost [portfolio](../../../../../../investment-portfolio.md), $\lambda_0$ is that [portfolio](../../../../../../investment-portfolio.md)'s certain return; if a [risk-free asset](../../../../../../risk-free-asset.md) is explicitly traded, [law of one price](../../../../../../law-of-one-price.md) makes it the [risk-free asset](../../../../../../risk-free-asset.md)'s return. No equilibrium preferences are needed for this argument.

## ↑ Ancestors (11)

1. [A](../a.md)
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
