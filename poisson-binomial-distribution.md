# Poisson binomial distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_binomial_distribution)

The sum of [independent](independent-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) with possibly unequal success [probabilities](probability.md) $p_i$ has a Poisson binomial distribution. Its [probability generating function](probability-generating-function.md) is $G_K(z)=\prod_i(1-p_i+p_i z)$: expand the product to read off the [probability mass function](probability-mass-function.md). [Linearity of expectation](linearity-of-expectation.md) and additivity of [variance](variance-split.md) for [independent random variables](independent-random-variables.md) give $\mathbb EK=\sum_i p_i$ and $\operatorname{Var}(K)=\sum_i p_i(1-p_i)$. Equal $p_i=p$ recover the [binomial distribution](binomial-distribution.md).

For three trials with success [probabilities](probability.md) $1/10,3/10,4/5$, expanding $(9/10+z/10)(7/10+3z/10)(1/5+4z/5)$ gives masses $0.126,0.572,0.278,0.024$ at $0,1,2,3$. Their [expected value](expected-value.md) is $1.2$ and [variance](variance-split.md) is $0.46$. Replacing all three success [probabilities](probability.md) by their average $0.4$ preserves the [expected value](expected-value.md) but gives [binomial distribution](binomial-distribution.md) [variance](variance-split.md) $0.72$, so it does not preserve the law.

## ↑ Ancestors (7)

1. [Discrete probability distribution](discrete-probability-distribution-split.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binomial distribution](binomial-distribution.md)
