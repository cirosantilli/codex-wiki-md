# Second-moment bound for positivity

↑ **Parent:** [Second moment method](second-moment-method.md)

For a nonnegative [random variable](random-variable-split.md) $N$ with positive [expected value](expected-value-split.md) and finite [second moment](second-moment.md), write $N=N\mathbf1_{\{N>0\}}$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives

$$
(\mathbb EN)^2=\left(\mathbb E[N\mathbf1_{\{N>0\}}]\right)^2\leq\mathbb E N^2\,\mathbb P(N>0),
$$

which proves the bound in [second moment method](second-moment-method.md). It is the zero-threshold case of the [Paley-Zygmund inequality](paley-zygmund-inequality.md). Equality occurs when $N$ is a fixed positive value on the [event](event.md) $N>0$ and zero elsewhere, [almost surely](almost-sure-convergence.md). For $N=10B$ with $B$ a [Bernoulli random variable](bernoulli-distribution.md) of parameter $1/10$, $(\mathbb EN)^2/\mathbb E N^2=1/10$ equals the exact positivity probability.

The [variance](variance-split.md) identity $\mathbb E N^2=(\mathbb EN)^2+\operatorname{Var}(N)$ turns the lower bound into a statement about variance relative to the squared [mean](expected-value-split.md). A small ratio forces positivity to be likely. A positive [expected value](expected-value-split.md) alone does not do so: keeping $\mathbb EN=1$ while taking $N=1/q$ with [probability](probability.md) $q$ and zero otherwise makes the positivity probability as small as any chosen $q>0$.

## ↑ Ancestors (7)

1. [Second moment method](second-moment-method.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Second moment method](second-moment-method.md)
