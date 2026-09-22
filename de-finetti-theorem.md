# De Finetti theorem

↑ **Parent:** [Exchangeable random variables](exchangeable-random-variables.md)

For an infinite sequence of real [exchangeable random variables](exchangeable-random-variables.md), conditional on its [invariant sigma-algebra of an exchangeable sequence](invariant-sigma-algebra-of-an-exchangeable-sequence.md), the coordinates are independent and identically distributed. In particular, for Borel sets $A_0,\ldots,A_p$,

$$
\mathbb E\!\left[\prod_{k=0}^p\mathbf1_{A_k}(X_k)\mid\mathcal S\right]
=\prod_{k=0}^p\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S].
$$

Here is the core proof. Let $\mathcal S_m$ denote invariance under permutations of coordinates $0,\ldots,m$. [Symmetrization as conditional expectation](symmetrization-as-conditional-expectation.md) identifies the empirical average of each indicator with its conditional expectation on $\mathcal S_m$. The [reverse martingale convergence theorem](reverse-martingale-convergence-theorem.md) gives its limit conditional on $\mathcal S$. Multiplying the averages sums over all ordered coordinate tuples, including repetitions. Symmetrization of the product itself sums over the distinct tuples. The fraction of repeated tuples is at most $\binom{p+1}{2}/(m+1)$, so these bounded averages have the same limit. This proves the displayed factorization. Permutation invariance also makes the individual conditional laws identical. A regular conditional distribution on the real line packages that common law as a random probability measure, giving the equivalent mixture-of-iid formulation.

## ↑ Ancestors (8)

1. [Exchangeable random variables](exchangeable-random-variables.md)
2. [Joint probability distribution](joint-probability-distribution.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/4/c/solution.md)
- [Sampling with and without replacement comparison for bounded products](sampling-with-and-without-replacement-comparison-for-bounded-products.md)
