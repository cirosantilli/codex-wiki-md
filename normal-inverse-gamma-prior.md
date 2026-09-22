# Normal-inverse-gamma prior

↑ **Parent:** [Conjugate prior](conjugate-prior.md)

For a [normal linear model](normal-linear-model.md) with coefficient vector $\eta$ and residual [variance](variance-split.md) $\sigma^2$, a normal-inverse-gamma prior has $\eta\mid\sigma^2\sim N(m,\sigma^2V)$ and $\sigma^2\sim\operatorname{IG}(a,b)$, with $V$ a [positive-definite matrix](positive-definite-matrix.md) and $a,b>0$. The inverse-gamma density is proportional to $(\sigma^2)^{-a-1}e^{-b/\sigma^2}$. Multiplying by the [normal linear model](normal-linear-model.md) [likelihood function](likelihood-function.md) and completing the square preserves the family, giving an analytic posterior and evidence integral.

## ↑ Ancestors (8)

1. [Conjugate prior](conjugate-prior.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/2/b/iii/solution.md)
