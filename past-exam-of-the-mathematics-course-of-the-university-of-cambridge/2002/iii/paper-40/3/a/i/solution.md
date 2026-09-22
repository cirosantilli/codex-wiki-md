<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a target [probability density function](../../../../../../../probability-density-function.md) $\pi(\theta_1,\ldots,\theta_p)$, one systematic sweep of the [Gibbs sampler](../../../../../../../gibbs-sampler.md) updates coordinates successively:

$$
\theta_j^{(m+1)}\sim\pi\left(\theta_j\mid\theta_1^{(m+1)},\ldots,\theta_{j-1}^{(m+1)},\theta_{j+1}^{(m)},\ldots,\theta_p^{(m)}\right),\quad j=1,\ldots,p.
$$

Each update leaves the target invariant: keeping the other coordinates with their target marginal and replacing one coordinate by its [conditional distribution](../../../../../../../conditional-distribution.md) reconstructs the target [joint probability density function](../../../../../../../joint-probability-density.md). Therefore composition of the coordinate updates also preserves $\pi$. It defines a [Markov chain](../../../../../../../markov-chain.md) whose consecutive draws are generally dependent. Under irreducibility, aperiodicity and the usual recurrence conditions it converges to the target law from an arbitrary valid start; a stationary start gives exact target marginals immediately. Invariance alone does not prove these ergodicity conditions, and a systematic full sweep need not itself be reversible.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
