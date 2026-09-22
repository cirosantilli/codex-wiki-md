# Poisson characterization by independent binomial splitting

↑ **Parent:** [Poisson thinning](poisson-thinning.md)

Let $N$ be a nonnegative integer-valued [random variable](random-variable-split.md) with finite [expected value](expected-value.md) $\mu$, and independently label each of its items with either of two equally likely labels. If the two resulting counts are [independent random variables](independent-random-variables.md), then $N$ has a [Poisson distribution](poisson-distribution.md). Indeed, its [probability generating function](probability-generating-function.md) obeys $G(s)=G((1+s)/2)^2$. With $H(t)=G(1-t)$, iteration gives $H(t)=H(t/2^k)^{2^k}$. Finite [expected value](expected-value.md) gives $H(h)=1-\mu h+o(h)$, hence $H(t)=e^{-\mu t}$ and $G(s)=e^{\mu(s-1)}$. Conversely, [Poisson thinning](poisson-thinning.md) produces independent [Poisson distributions](poisson-distribution.md) for the two counts.

## ↑ Ancestors (7)

1. [Poisson thinning](poisson-thinning.md)
2. [Poisson process](poisson-process.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/10f/c/solution.md)
