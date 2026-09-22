<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the target posterior density as $\pi(\theta)$ and the [proposal distribution](../../../../../../proposal-distribution.md) density as $q(\theta'\mid\theta)$. The [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) accepts a proposed move with

$$
a(\theta,\theta')=
\min\!\left\{1,
\frac{\pi(\theta')q(\theta\mid\theta')}
{\pi(\theta)q(\theta'\mid\theta)}\right\}.
$$

For distinct states,

$$
\pi(\theta)q(\theta'\mid\theta)a(\theta,\theta')
=\min\{\pi(\theta)q(\theta'\mid\theta),
\pi(\theta')q(\theta\mid\theta')\},
$$

which is symmetric in $\theta$ and $\theta'$. The rejection probability supplies the diagonal part, so the entire transition kernel satisfies [detailed balance](../../../../../../detailed-balance.md). Integrating the detailed-balance identity over the starting state proves $\int\pi(\theta)P(\theta,d\theta')=\pi(\theta')d\theta'$. Hence the posterior is a [stationary distribution](../../../../../../stationary-distribution.md); an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) that is also an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md) converges uniquely to it.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
