<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First require a proper target: $0<Z=\int_{\mathbb R^d}\pi(x)\,dx<\infty$ and $\bar\pi=\pi/Z$. The [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) uses the [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md)

$$
a(x,y)=\min\!\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.
$$

Sufficient general conditions are [phi-irreducibility](../../../../../../phi-irreducibility.md), [aperiodicity](../../../../../../aperiodic-markov-chain.md), and a [drift-minorisation condition](../../../../../../drift-minorisation-condition.md) establishing [geometric ergodicity](../../../../../../geometric-ergodicity.md) of the resulting chain, together with a stationary $(2+\delta)$th moment for the observable being averaged. These imply the [central limit theorem for a geometrically ergodic Markov chain](../../../../../../central-limit-theorem-for-a-geometrically-ergodic-markov-chain.md). The observable's moment condition must be included: conditions on the sampler alone cannot give the theorem for every arbitrary function.

A concrete stronger condition, directly in terms of the proposal, is

$$
\boxed{q(y\mid x)\geq\epsilon\bar\pi(y)\quad\text{for all }x,y\text{ in the target support},\qquad\epsilon>0.}
$$

Together with a bounded observable, this is an especially simple sufficient answer. The accepted proposal density is $\min\{q(y\mid x),\bar\pi(y)q(x\mid y)/\bar\pi(x)\}$, so it is at least $\epsilon\bar\pi(y)$. The kernel satisfies a global [minorization condition](../../../../../../minorization-condition.md) with the target, hence [uniform geometric ergodicity](../../../../../../uniform-geometric-ergodicity.md), positive [Harris recurrence](../../../../../../harris-recurrent-markov-chain.md), and [aperiodicity](../../../../../../aperiodic-markov-chain.md). An independent proposal whose importance weight $\bar\pi(y)/q(y)$ is uniformly bounded is one example. No claim of these properties follows merely from writing down a positive proposal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
