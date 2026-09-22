# Exact factor pricing without a traded risk-free asset

↑ **Parent:** [Arbitrage pricing theory](arbitrage-pricing-theory.md)

Suppose [asset returns](financial-return.md) have the exact representation $r=a+Bf$, allowing unrestricted long and short [portfolios](investment-portfolio.md). A position $v$ with $\mathbf1^Tv=0$ and $B^Tv=0$ costs zero and has constant [financial payoff](contingent-claim-payoff.md) $a^Tv$. Absence of [arbitrage](arbitrage.md) therefore forces $a^Tv=0$, since either sign of $v$ is allowed. The [orthogonal complement](orthogonal-complement.md) identity gives $a\in\operatorname{span}(\mathbf1,\operatorname{col}B)$. Taking [expectations](expected-value.md) proves the displayed pricing relation, with $\lambda$ equal to the coefficients of $B$ in $a$ plus $\mathbb E f$. When $[\mathbf1\ B]$ has full column [rank](rank-one-quadratic-form.md), $\lambda_0$ is the return of a unit-cost zero-exposure [portfolio](investment-portfolio.md) and $\lambda_j$ is the [expected return](expected-return.md) of a zero-cost [portfolio](investment-portfolio.md) with exposure one to factor $j$ and zero to the others. Without that [rank](rank-one-quadratic-form.md) condition the coefficients need not be unique, and a traded zero-exposure [portfolio](investment-portfolio.md) need not exist.

## ↑ Ancestors (7)

1. [Arbitrage pricing theory](arbitrage-pricing-theory.md)
2. [Arbitrage](arbitrage.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/2/a/solution.md)
