# Thinning of a Markov chain

↑ **Parent:** [Markov chain Monte Carlo](markov-chain-monte-carlo.md)

Thinning keeps every $L$th state of a [Markov chain](markov-chain.md). The retained chain has transition kernel $K^L$ and the same stationary distribution. It is generally still dependent, and reducing correlation between retained draws does not by itself improve precision per original transition. Keep all post-warmup draws unless storage or later processing requires thinning; assess precision using the [effective sample size of a Markov chain](effective-sample-size-of-a-markov-chain.md).

## ↑ Ancestors (7)

1. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/2/iv/solution.md)
