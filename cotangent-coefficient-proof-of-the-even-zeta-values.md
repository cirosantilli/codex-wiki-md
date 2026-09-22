# Cotangent coefficient proof of the even zeta values

↑ **Parent:** [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md)

The [cotangent partial-fraction expansion](cotangent-partial-fraction-expansion.md) gives, on $0<|z|<1$,

$$
\pi\cot(\pi z)=z^{-1}-2\sum_{r\geq1}\zeta(2r)z^{2r-1}.
$$

The [Bernoulli number](bernoulli-number-split.md) [generating function](generating-function.md) gives the same [Laurent series](laurent-series.md) in another form:

$$
\pi\cot(\pi z)=\pi i+\frac{2\pi i}{e^{2\pi iz}-1}
=z^{-1}+\sum_{r\geq1}\frac{B_{2r}(2\pi i)^{2r}}{(2r)!}z^{2r-1}.
$$

The $B_1$ term cancels the separate $\pi i$; the higher odd [Bernoulli numbers](bernoulli-number-split.md) vanish. Comparing [Laurent coefficients](laurent-coefficient.md) therefore gives $-2\zeta(2r)=B_{2r}(2\pi i)^{2r}/(2r)!$, which is the stated real formula because $i^{2r}=(-1)^r$. The [cotangent partial-fraction expansion](cotangent-partial-fraction-expansion.md) justifies the convergent expansion before the [coefficient](coefficient.md) comparison; a finite plot of [partial sums](partial-sum.md) alone would not prove the infinite identity.

## ↑ Ancestors (6)

1. [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md)
2. [Bernoulli number](bernoulli-number-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Basel problem](basel-problem.md)
