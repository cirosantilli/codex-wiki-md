<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Both the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) and the [Gibbs sampler](../../../../../../gibbs-sampler.md) construct a [Markov chain](../../../../../../markov-chain.md) with a specified target distribution, usually a [posterior distribution](../../../../../../bayesian-posterior.md) known only up to normalization. For a proposal density $q(y\mid x)$ and target density $\pi$, the [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) is

$$
a(x,y)=\min\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.
$$

After drawing $y$, move there with this probability; otherwise stay at $x$. The unknown normalizing constant of $\pi$ cancels. The original Metropolis algorithm uses a symmetric proposal, $q(y\mid x)=q(x\mid y)$, so the proposal-density ratio disappears. The general [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) permits nonsymmetric proposals and needs that correction.

A [Gibbs sampler](../../../../../../gibbs-sampler.md) instead chooses a coordinate or block and draws directly from its [full conditional distribution](../../../../../../full-conditional-distribution.md), leaving the other coordinates fixed. It is exactly a conditional Metropolis–Hastings update whose proposal is that full conditional. For a change from $x_i$ to $y_i$ with $x_{-i}$ fixed, the acceptance ratio is

$$
\frac{\pi(y_i,x_{-i})\pi(x_i\mid x_{-i})}{\pi(x_i,x_{-i})\pi(y_i\mid x_{-i})}=1.
$$

Thus **a Gibbs update is an always-accepted Metropolis–Hastings update with the full conditional as proposal**. This statement concerns each update: a systematic sweep of several Gibbs kernels preserves the target but need not itself be reversible.

When the [full conditional distributions](../../../../../../full-conditional-distribution.md) are easy to sample, a [Gibbs sampler](../../../../../../gibbs-sampler.md) avoids proposal tuning and rejection, and is particularly convenient for [conjugate priors](../../../../../../conjugate-prior.md) and [data augmentation](../../../../../../data-augmentation.md). When a conditional cannot be sampled directly, a [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) can use only its evaluable density; such an update can also be inserted into a Gibbs sweep. Block or joint Metropolis–Hastings proposals can move efficiently along strongly correlated directions for which coordinate-wise Gibbs updates mix slowly. Conversely, a badly chosen Metropolis–Hastings proposal can reject most moves or make only tiny moves. Acceptance probability one by itself does not guarantee rapid exploration. Both methods require appropriate irreducibility and convergence checks before their long-run averages are useful posterior estimates.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
