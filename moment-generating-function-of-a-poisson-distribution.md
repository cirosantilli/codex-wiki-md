# Moment-generating function of a Poisson distribution

↑ **Parent:** [Poisson distribution](poisson-distribution.md)

For $N\sim\operatorname{Pois}(\lambda)$ with $\lambda\geq0$, insert its [probability mass function](probability-mass-function.md) into the [expected value](expected-value-split.md):

$$
\mathbb E e^{tN}=e^{-\lambda}\sum_{j\geq0}\frac{(\lambda e^t)^j}{j!}
=\exp(\lambda(e^t-1)),\qquad t\in\mathbb R.
$$

The [exponential series](exponential-series.md) shows finiteness for every real $t$. Differentiating this [moment-generating function](moment-generating-function.md) gives [mean](expected-value-split.md) and [variance](variance-split.md) both $\lambda$. Taking the [logarithm](logarithm.md) gives the [cumulant-generating function](cumulant-generating-function.md) $\lambda(e^t-1)$, so every positive-order [cumulant](cumulant.md) is also $\lambda$.

## ↑ Ancestors (8)

1. [Poisson distribution](poisson-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/1/b/ii/solution.md)
- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/1/c/i/solution.md)
