# Integer coefficients with a prescribed radius of convergence

↑ **Parent:** [Radius of convergence](radius-of-convergence.md)

Every $R\in[0,1]$ occurs as the [radius of convergence](radius-of-convergence.md) of a [power series](power-series.md) all of whose [coefficients](coefficient.md) are positive [integers](integer-split.md). For $0<R\leq1$, use the [ceiling function](ceiling-function.md) to choose $a_n=\lceil R^{-n}\rceil$. Then

$$
R^{-n}\leq a_n< R^{-n}+1\leq2R^{-n}.
$$

For $|z|<R$, the [comparison test for series](comparison-test-for-series.md) with a [geometric series](geometric-series.md) proves [absolute convergence](absolute-convergence.md). For $|z|\geq R$, the bound $|a_nz^n|\geq(|z|/R)^n\geq1$ violates the fact that [terms of a convergent series tend to zero](terms-of-a-convergent-series-tend-to-zero.md). Hence the [radius of convergence](radius-of-convergence.md) is exactly $R$.

For $R=0$, use $a_n=n!$: at every $z\ne0$ the ratio of successive term [absolute values](absolute-value.md) is $(n+1)|z|$, eventually exceeding two. The [factorial](factorial.md) [coefficients](coefficient.md) therefore give divergence away from zero.

A [power series](power-series.md) with every [coefficient](coefficient.md) a positive [integer](integer-split.md) cannot have [radius of convergence](radius-of-convergence.md) greater than one: $a_n\geq1$ makes convergence impossible at $z=1$. If zero [coefficients](coefficient.md) are allowed and only finitely many are nonzero, a [polynomial](polynomial-split.md) instead has infinite [radius of convergence](radius-of-convergence.md).

## ↑ Ancestors (8)

1. [Radius of convergence](radius-of-convergence.md)
2. [Power series](power-series.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
