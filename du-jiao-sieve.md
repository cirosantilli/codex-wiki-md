# Du Jiao sieve

↑ **Parent:** [Number-theoretic sieve](number-theoretic-sieve.md)

A Du Jiao sieve computes a summatory [arithmetic function](arithmetic-function-split.md) using a [Dirichlet convolution](dirichlet-convolution.md) identity and [memoization](memoization.md) of repeated quotient arguments. For the [Mertens function](mertens-function.md) $M(n)=\sum_{k\le n}\mu(k)$, the identity $\sum_{d\mid k}\mu(d)=[k=1]$ gives $M(n)=1-\sum_{i=2}^n M(\lfloor n/i\rfloor)$. Grouping equal quotients and precomputing small arguments makes this [recurrence relation](recurrence-relation.md) useful for large inputs.

## ↑ Ancestors (4)

1. [Number-theoretic sieve](number-theoretic-sieve.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
