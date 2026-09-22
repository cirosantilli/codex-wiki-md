<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a target [probability density function](../../../../../../probability-density-function.md) $\pi$ and a [proposal distribution](../../../../../../proposal-distribution.md) with density $q(x'\mid x)$, the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) starts in the target support and repeats: propose $x'\sim q(\cdot\mid x)$, draw an [independent](../../../../../../independent-random-variables.md) uniform $U$, and move to $x'$ if

$$
U\le\alpha(x,x'),\qquad\boxed{\alpha(x,x')=\min\left(1,\frac{\pi(x')q(x\mid x')}{\pi(x)q(x'\mid x)}\right).}
$$

Otherwise retain $x$. A zero reverse-proposal density makes the acceptance zero. Unknown multiplicative constants of $\pi$ cancel. For distinct states,

$$
\pi(x)q(x'\mid x)\alpha(x,x')=\min\{\pi(x)q(x'\mid x),\pi(x')q(x\mid x')\},
$$

which is symmetric in the states. Together with the probability of holding at the current state, this proves [detailed balance](../../../../../../detailed-balance.md) and invariance of $\pi$. Successive values form a dependent [Markov chain](../../../../../../markov-chain.md); convergence from arbitrary initial states additionally needs the appropriate irreducibility and [aperiodicity](../../../../../../aperiodic-markov-chain.md), not just this invariant-density identity.

The [Gibbs sampler](../../../../../../gibbs-sampler.md) updates a coordinate using its [full conditional distribution](../../../../../../full-conditional-distribution.md) while keeping the others fixed. For coordinate $i$, write $r=x_{-i}$ and $\pi(x)=\pi_{-i}(r)\pi_i(x_i\mid r)$. Its proposal replaces $x_i$ by $x_i'\sim\pi_i(\cdot\mid r)$. The MH ratio, interpreted on this one-coordinate proposal space, is

$$
\frac{\pi_{-i}(r)\pi_i(x_i'\mid r)\pi_i(x_i\mid r)}{\pi_{-i}(r)\pi_i(x_i\mid r)\pi_i(x_i'\mid r)}=1.
$$

Thus **every Gibbs coordinate update is an MH update with acceptance one**. A random choice of coordinate gives a mixture of these invariant kernels; a deterministic sweep gives their composition. Both preserve $\pi$. The latter composition need not be reversible, so the special-case statement is about the coordinate kernels, not a claim that every entire systematic sweep is one reversible MH kernel.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
