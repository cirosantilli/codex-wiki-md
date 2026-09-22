<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A systematic [Gibbs sampler](../../../../../../../gibbs-sampler.md) updates the coordinates of $\theta$ successively from their [full conditional distributions](../../../../../../../full-conditional-distribution.md). At iteration $t$, draw

$$
\theta_j^{(t+1)}\sim\pi\left(\theta_j\mid
\theta_1^{(t+1)},\ldots,\theta_{j-1}^{(t+1)},
\theta_{j+1}^{(t)},\ldots,\theta_p^{(t)}\right),\qquad j=1,\ldots,p.
$$

For a single coordinate, if the current state has distribution $\pi$, its untouched coordinates have the correct marginal law and the resampled coordinate has precisely the conditional law under $\pi$. Integrating marginal times conditional therefore recovers $\pi$. Each coordinate kernel preserves this [invariant distribution](../../../../../../../stationary-distribution.md), so their composition also preserves it. This proves the target of the [Gibbs sampler](../../../../../../../gibbs-sampler.md); the whole systematic sweep need not be a reversible kernel.

Starting from a suitable state and assuming the required irreducibility and convergence conditions, discard an initial transient and retain subsequent states as a dependent sample from, or approximately from, $\pi$. In finite-state problems irreducibility and aperiodicity suffice; in continuous-state problems the corresponding positive recurrence and ergodicity conditions must hold. Successive draws are generally dependent, so Monte Carlo uncertainty must account for that dependence.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
