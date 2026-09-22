<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Variational inference](../../../../../variational-inference.md) replaces exact [Bayesian inference](../../../../../bayesian-statistics-split.md) by an [optimization](../../../../../mathematical-optimization-split.md) problem over a tractable family $q_\lambda(z)$. A [guide program](../../../../../guide-program.md) samples from this approximating family. Optimizing an [evidence lower bound](../../../../../evidence-lower-bound.md) is equivalent to minimizing $D_{\rm KL}(q_\lambda\Vert p(\cdot\mid x))$. Its appeal is that a fitted approximation can be cheap to sample and may scale well when an exact [posterior distribution](../../../../../bayesian-posterior.md) is inaccessible. A restricted family, such as [mean-field variational inference](../../../../../mean-field-variational-inference.md), can miss dependence or entire modes; a local optimum can add further error. More optimization cannot remove approximation error caused by an inadequate family.

[Monte Carlo method](../../../../../monte-carlo-method-split.md) inference instead estimates posterior [expectations](../../../../../expected-value-split.md) using simulated values or weighted values. Examples include [rejection sampling](../../../../../rejection-sampling.md), [importance sampling](../../../../../importance-sampling.md) and [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md). Under their respective support and convergence assumptions, increasing computation can yield consistent estimates without choosing a finite-dimensional posterior family. Their uncertainty includes simulation error; an inefficient proposal or slow [mixing time](../../../../../mixing-time-of-a-markov-chain.md) can make that error large. [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md) additionally requires convergence and dependence diagnostics.

**The central trade-off is optimization within an approximate family versus simulation under a target [probability distribution](../../../../../probability-distribution-split.md).** It is not an absolute distinction between deterministic and random computation: [variational inference](../../../../../variational-inference.md) often uses [Monte Carlo method](../../../../../monte-carlo-method-split.md) estimates of its [gradient](../../../../../gradient.md), while [Monte Carlo method](../../../../../monte-carlo-method-split.md) inference may use fitted proposals. Neither method automatically guarantees accurate uncertainty estimates or superiority at a fixed computational budget.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
