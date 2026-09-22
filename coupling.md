# Coupling

↑ **Parent:** [Probability and statistics](probability-and-statistics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coupling_(probability))

A [coupling of probability distributions](coupling.md) $\mu,\nu$ is a [joint probability distribution](joint-probability-distribution.md) of [random variables](random-variable-split.md) $(X,Y)$ whose [marginal distributions](marginal-distribution.md) are $\mu,\nu$. It lets us choose the [statistical dependence](statistical-dependence.md) between two random constructions while preserving the individual laws. This choice can make a comparison much easier: giving two simulations the same random input may keep their paths close, even though separately generating both paths would hide that relationship.[§4.2, coupling definition and Example 4.6, printed pp. 49–50](markov-chains-and-mixing-times-second-edition-by-david-a-levin-and-others.md)

For example, two fair coin tosses can be generated independently, with mismatch [probability](probability.md) $1/2$, or by tossing once and setting $Y=X$, with mismatch [probability](probability.md) zero. Both constructions have the same two [Bernoulli distributions](bernoulli-distribution.md) as marginals. Their joint laws differ. A [maximal coupling](maximal-coupling.md) makes the values agree as often as possible; a [coalescing coupling](coalescing-coupling.md) arranges permanent agreement of two processes after a random time. Minimizing expected geometric separation instead leads to [Wasserstein distance](wasserstein-distance.md).

**Table of contents**

- [Summable-memory coupling](summable-memory-coupling.md)
- [Eventual coupling of planar symmetric random walks](eventual-coupling-of-planar-symmetric-random-walks.md)
- [Stochastic domination of probability measures](stochastic-domination-of-probability-measures.md)
  - [Holley inequality](holley-inequality.md)
    - [Holley condition](holley-condition.md)
- [Synchronous coupling](synchronous-coupling.md)
  - [Mean-square contraction of synchronously coupled diffusions](mean-square-contraction-of-synchronously-coupled-diffusions.md)
    - [A bounded drift cannot be uniformly strictly dissipative on the real line](a-bounded-drift-cannot-be-uniformly-strictly-dissipative-on-the-real-line.md)
    - [Convergence by synchronous coupling for bounded continuous test functions](convergence-by-synchronous-coupling-for-bounded-continuous-test-functions.md)
- [Coalescing coupling](coalescing-coupling.md)
  - [Mirror coupling under an involution](mirror-coupling-under-an-involution.md)
- [Bernoulli coupling by a shared uniform random variable](bernoulli-coupling-by-a-shared-uniform-random-variable.md)
- [Maximal coupling](maximal-coupling.md)
- [Wasserstein distance](wasserstein-distance.md)
  - [Displacement interpolation](displacement-interpolation.md)
  - [Kantorovich–Rubinstein theorem](kantorovich-rubinstein-theorem.md)
    - [Lipschitz regularization of transport potentials](lipschitz-regularization-of-transport-potentials.md)
  - [p-Wasserstein distance](p-wasserstein-distance.md)
  - [Second Wasserstein distance](second-wasserstein-distance.md)
    - [One-dimensional second-Wasserstein convergence criterion](one-dimensional-second-wasserstein-convergence-criterion.md)
  - [Wasserstein contraction](wasserstein-contraction.md)

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Coupling characterization of total variation distance](coupling-characterization-of-total-variation-distance.md)
- [Coupling inequality for total variation](coupling-inequality-for-total-variation.md)
- [Maximal coupling](maximal-coupling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/5/ii/solution.md)
