<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At temperature $T>0$, target a [probability density function](../../../../../../../probability-density-function.md) proportional to $\exp(f(\theta)/T)$ on a parameter region where it is normalizable, possibly with a specified proper base measure. A [Metropolis–Hastings algorithm](../../../../../../../metropolis-hastings-algorithm.md) proposal $q(\theta,\theta')$ has acceptance [probability](../../../../../../../probability.md)

$$
\min\left\{1,\exp\left[\frac{f(\theta')-f(\theta)}T\right]\frac{q(\theta',\theta)}{q(\theta,\theta')}\right\}.
$$

For a symmetric proposal, improving moves are accepted and a loss $\Delta$ is accepted with [probability](../../../../../../../probability.md) $e^{-\Delta/T}$. Run updates while gradually lowering $T$ toward zero. This [simulated annealing](../../../../../../../simulated-annealing.md) scheme initially permits exploration and increasingly favors high objective values. Appropriate cooling and mixing conditions are needed for a general global convergence theorem; a finite arbitrary schedule does not guarantee finding a global maximum.

To maximize a positive [likelihood function](../../../../../../../likelihood-function.md), take $f=\log L$, which has the same maximizers. The resulting [likelihood-power annealing](../../../../../../../likelihood-power-annealing.md) target is $L^{1/T}$, and available [Gibbs sampler](../../../../../../../gibbs-sampler.md) [conditional distributions](../../../../../../../conditional-distribution.md) can replace Metropolis proposals.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
