<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md), start at a state $\theta$ with positive target density, propose $\theta'$ from $q(\theta'\mid\theta)$, and generate an independent uniform draw. Accept the proposal with probability

$$
\boxed{\alpha(\theta,\theta')=\min\left\{1,
\frac{\pi(\theta')q(\theta\mid\theta')}{\pi(\theta)q(\theta'\mid\theta)}\right\}.}
$$

On rejection retain $\theta$, including repeated states in the chain; removing repeats would generally change its stationary law. The accepted-flow density satisfies

$$
\pi(\theta)q(\theta'\mid\theta)\alpha(\theta,\theta')
=\min\{\pi(\theta)q(\theta'\mid\theta),\pi(\theta')q(\theta\mid\theta')\},
$$

which is symmetric in its two states. This proves [detailed balance](../../../../../../detailed-balance.md) and hence invariance of the target distribution, including the holding probabilities on the diagonal. Unknown common normalization constants cancel in the ratio. Invariance alone does not establish convergence from arbitrary initial states. Choosing proposals that yield a [positive Harris recurrent Markov chain](../../../../../../positive-harris-recurrent-markov-chain.md) with [aperiodicity](../../../../../../aperiodic-markov-chain.md) supplies the usual convergence guarantee, and the resulting sample is dependent. Use burn-in and account for autocorrelation when assessing Monte Carlo precision.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
