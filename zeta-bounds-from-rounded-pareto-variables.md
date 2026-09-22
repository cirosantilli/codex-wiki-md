# Zeta bounds from rounded Pareto variables

↑ **Parent:** [Pareto distribution](pareto-distribution.md)

Let $X$ have [survival function](survival-function.md) $\mathbb P(X\ge x)=x^{-s}$ for $x\ge1$, with $s>1$. Its [expected value](expected-value-split.md) is $s/(s-1)$. The [tail-sum formula for expectation](tail-sum-formula-for-expectation.md) gives

$$
\mathbb E[\lfloor X\rfloor]=\sum_{k\ge1}k^{-s}=\zeta(s).
$$

The [absolutely continuous probability distribution](absolutely-continuous-probability-distribution.md) gives zero mass to the [integers](integer-split.md), so $\lceil X\rceil=\lfloor X\rfloor+1$ almost surely and $\mathbb E[\lceil X\rceil]=\zeta(s)+1$. Taking expectations of $\lfloor X\rfloor\le X\le\lceil X\rceil$ gives $\zeta(s)\le s/(s-1)\le\zeta(s)+1$, which rearranges to the displayed bounds on the [Riemann zeta function](riemann-zeta-function.md). Finiteness is justified by $\lfloor X\rfloor\le X$ and $\lceil X\rceil\le X+1$.

## ↑ Ancestors (8)

1. [Pareto distribution](pareto-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/9/b/v/solution.md)
