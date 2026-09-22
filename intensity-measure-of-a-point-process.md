# Intensity measure of a point process

↑ **Parent:** [Point process](point-process.md)

The [intensity measure of a point process](intensity-measure-of-a-point-process.md) $\Pi$ is its expected counting [measure](measure-split.md):

$$
\mu(A)=\mathbb E[\Pi(A)],\qquad A\in\mathcal B(E).
$$

It may take the value $+\infty$.[Section 2.2, Definition 2.5, printed p. 12: intensity as the expected counting measure](lectures-on-the-poisson-process-by-gunter-last-and-others.md) Countable additivity follows by applying the [monotone convergence theorem](monotone-convergence-theorem.md) to the counts of finite unions of pairwise [disjoint observation windows](disjoint-observation-windows.md). If $\mu$ is locally finite and [absolutely continuous with respect to](absolute-continuity-of-measures.md) [Lebesgue measure](lebesgue-measure.md), its [Radon-Nikodym derivative](radon-nikodym-derivative.md) is the [intensity function of a point process](intensity-function-of-a-point-process.md) $\lambda$:

$$
\mu(A)=\int_A\lambda(x)\,dx.
$$

This is an expected number per unit volume, not a [probability density function](probability-density-function.md) for a randomly selected point. For example, a single deterministic point has $\mu=\delta_0$, a [Dirac measure](dirac-measure.md), and no [Lebesgue measure](lebesgue-measure.md) density. The density representation requires its own assumption.[Section 2.1, Definitions 2.1-2.2, printed pp. 26-27: expected counts and intensity functions](stochastic-geometry-lectures-given-at-the-c-i-m-e-summer-school-held-in-martina-franca-italy-september-13-18-2004/spatial-point-processes-and-their-applications.md)

For a bounded [Borel set](borel-set.md) $W$, $\mathbb E[N_W]=\mu(W)$, but local finiteness alone does not ensure that this [expected value](expected-value-split.md) is finite. Conversely, $\mu(W)<\infty$ implies $N_W<\infty$ [almost surely](almost-sure-convergence.md), even when $W$ is unbounded. A constant finite [intensity function of a point process](intensity-function-of-a-point-process.md) on all of $\mathbb R^d$ has infinite total [intensity measure](intensity-measure-of-a-point-process.md), although every bounded window has finite [expected value](expected-value-split.md).

**Table of contents**

- [Local finiteness does not imply finite intensity](local-finiteness-does-not-imply-finite-intensity.md)
- [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)
  - [Randomly shifted lattice point process](randomly-shifted-lattice-point-process.md)
  - [Shared random rate gives dependent point counts](shared-random-rate-gives-dependent-point-counts.md)

## ↑ Ancestors (6)

1. [Point process](point-process.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Existence of a Poisson random measure on a standard Borel space](existence-of-a-poisson-random-measure-on-a-standard-borel-space.md)
- [Intensity measure of a point process](intensity-measure-of-a-point-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39/3/solution.md)
- [Point process](point-process.md)
