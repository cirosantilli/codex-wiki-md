# Truncated Euler-product lower bound

↑ **Parent:** [Euler product](euler-product.md)

For a finite set of [primes](prime-number.md) choose $0<g(p)<1$, put $k(p)=g(p)/(1-g(p))$, and let $W=\prod_p(1+k(p))$. Give each [squarefree integer](squarefree-integer.md) $d$ on these primes probability $k(d)/W$. Inclusion of each [prime](prime-number.md) is represented by a [Bernoulli random variable](bernoulli-distribution.md) with parameter $g(p)$; these are [independent random variables](independent-random-variables.md), so $\mathbb E[\log d]=\sum_pg(p)\log p$. If this is at most $\theta\log L$ with $0<\theta<1$, the [Markov inequality](markov-inequality.md) gives

$$
\sum_{d\leq L}k(d)\geq(1-\theta)W.
$$

This turns a full [Euler product](euler-product.md) into a lower bound for the truncated normalizing sum of a [Selberg sieve](selberg-sieve.md).

## ↑ Ancestors (7)

1. [Euler product](euler-product.md)
2. [Dirichlet series](dirichlet-series.md)
3. [Analytic number theory](analytic-number-theory-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Half-dimensional interval sieve](half-dimensional-interval-sieve.md)
- [Mertens first theorem](mertens-first-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/5/a/solution.md)
- [Twin-prime upper bound from a quadratic sieve](twin-prime-upper-bound-from-a-quadratic-sieve.md)
- [Twin-prime upper bound using Bombieri–Vinogradov](twin-prime-upper-bound-using-bombieri-vinogradov.md)
