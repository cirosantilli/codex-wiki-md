# Edgeworth series

↑ **Parent:** [Cumulant expansion](cumulant-expansion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edgeworth_series)

An Edgeworth expansion approximates a [probability density function](probability-density-function.md) by a [normal distribution](normal-distribution.md) multiplied by [Hermite polynomials](hermite-polynomial.md) encoding higher [cumulants](cumulant.md). For a centered variable of [variance](variance-split.md) $\sigma^2$ and third cumulant $\kappa_3$,

$$
p(x)=\frac{e^{-x^2/(2\sigma^2)}}{\sqrt{2\pi}\sigma}
\left[1+\frac{\kappa_3}{6\sigma^3}
\operatorname{He}_3(x/\sigma)+\cdots\right],
\qquad \operatorname{He}_3(z)=z^3-3z.
$$

The correction follows from inverse-transforming the cubic term of the [cumulant-generating function](cumulant-generating-function.md). It is an asymptotic approximation near the bulk of the distribution; truncation can give a negative result in far tails.

**Table of contents**

- [Symmetric Edgeworth coverage cancellation](symmetric-edgeworth-coverage-cancellation.md)
- [Cornish-Fisher expansion](cornish-fisher-expansion.md)

## ↑ Ancestors (9)

1. [Cumulant expansion](cumulant-expansion.md)
2. [Cumulant-generating function](cumulant-generating-function.md)
3. [Moment-generating function](moment-generating-function.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/6/i/solution.md)
