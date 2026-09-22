# Metropolis sampling on fixed-cardinality subsets

↑ **Parent:** [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)

Represent a size-$k$ subset of $n$ objects by a binary [vector](vector.md) with coordinate sum $k$, where $0<k<n$. Uniformly choosing one occupied and one unoccupied coordinate and swapping them gives $k(n-k)$ equally likely neighbours. This [proposal distribution](proposal-distribution.md) is symmetric, so its forward and reverse factors cancel in the [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md). Every state is connected to every other by a sequence of swaps, establishing an [irreducible Markov chain](irreducible-markov-chain.md) when the target masses are positive. Symmetry and the acceptance rule give [detailed balance](detailed-balance.md) with that target.

For a [discrete uniform distribution](discrete-uniform-distribution.md) as the [prior distribution](prior-probability.md) and a [multivariate normal distribution](multivariate-normal-distribution.md) for observations with [covariance matrix](covariance-matrix.md) $\Sigma$ and mean $u$, the [posterior distribution](bayesian-posterior.md) is proportional to $\exp[-(x-u)^T\Sigma^{-1}(x-u)/2]$. If $d=v-u$, expanding the [quadratic forms](quadratic-form-split.md) gives log acceptance ratio $d^T\Sigma^{-1}(x-u)-d^T\Sigma^{-1}d/2$, and the log acceptance [probability](probability.md) is its minimum with zero.

## ↑ Ancestors (8)

1. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/3/c/i/solution.md)
