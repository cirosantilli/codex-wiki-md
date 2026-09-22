# Recycling a uniform random variable after discrete sampling

↑ **Parent:** [Inverse transform sampling](inverse-transform-sampling.md)

For positive [mixture weights](mixture-weight.md) $w_j$ summing to one, set $C_j=\sum_{i\leq j}w_i$ and choose $J=j$ when $C_{j-1}\leq U<C_j$, where $U$ has a [uniform distribution](continuous-uniform-distribution.md). Then $V=(U-C_{J-1})/w_J$ has a [uniform distribution](continuous-uniform-distribution.md) independently of $J$: for $0\leq v\leq1$, $\Pr(J=j,V\leq v)=w_jv$. This permits exact [finite mixture model](finite-mixture-model.md) sampling with a recycled continuous [random variable](random-variable-split.md).

## ↑ Ancestors (8)

1. [Inverse transform sampling](inverse-transform-sampling.md)
2. [Quantile function](quantile-function.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/c/solution.md)
