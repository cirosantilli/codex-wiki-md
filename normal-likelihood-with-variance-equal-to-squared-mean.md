# Normal likelihood with variance equal to squared mean

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

For independent [normal distribution](normal-distribution.md) observations with mean $\mu>0$ and variance $\mu^2$, put $S_1=\sum_iX_i$, $S_2=\sum_iX_i^2$. The [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md) makes $(S_1,S_2)$ a [sufficient statistic](sufficient-statistic.md), since the [likelihood](likelihood-function.md) is proportional to $\mu^{-n}\exp[-S_2/(2\mu^2)+S_1/\mu]$. Its logarithmic [derivative](derivative.md) has numerator $S_2-S_1\mu-n\mu^2$. When $S_2>0$, this changes sign once on the positive half-line and gives the displayed global [maximum-likelihood estimator](maximum-likelihood-estimator.md). The zero sample is a probability-zero exception with unbounded [likelihood](likelihood-function.md) as $\mu\downarrow0$.

## ↑ Ancestors (7)

1. [Maximum likelihood estimation](maximum-likelihood-estimation.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/3d/solution.md)
