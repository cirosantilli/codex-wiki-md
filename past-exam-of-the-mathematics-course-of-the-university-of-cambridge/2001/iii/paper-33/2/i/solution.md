<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md), start at a point $x$ with positive target [probability density function](../../../../../../probability-density-function.md). Draw $Y$ from a proposal [probability density function](../../../../../../probability-density-function.md) $q(y\mid x)$, generate an [independent](../../../../../../independent-random-variables.md) [uniform distribution](../../../../../../continuous-uniform-distribution.md) value $U$, and set the next state to $Y$ if

$$
U\leq\alpha(x,Y),\qquad
\boxed{\alpha(x,y)=\min\!\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.}
$$

Otherwise retain $x$, including that repeated state in the sample. Where a proposed forward move is possible but its reverse [probability density function](../../../../../../probability-density-function.md) vanishes, its acceptance [probability](../../../../../../probability.md) is zero. Unknown [normalizing constants](../../../../../../normalizing-constant.md) in $\pi$ cancel.

For distinct states, the accepted [probability](../../../../../../probability.md) flow is

$$
\pi(x)q(y\mid x)\alpha(x,y)
=\min\{\pi(x)q(y\mid x),\pi(y)q(x\mid y)\},
$$

which is symmetric in $x,y$. This [detailed balance](../../../../../../detailed-balance.md) identity, together with the holding [probability](../../../../../../probability.md), proves that $\pi$ is invariant. Under appropriate irreducibility and aperiodicity conditions the chain converges to $\pi$; successive states are generally dependent.

The [Gibbs sampler](../../../../../../gibbs-sampler.md) updates coordinates from their [full conditional distributions](../../../../../../full-conditional-distribution.md). In a systematic sweep, draw successively

$$
X_j^{(r)}\sim
\pi\!\left(\,\cdot\mid X_1^{(r)},\ldots,X_{j-1}^{(r)},
X_{j+1}^{(r-1)},\ldots,X_k^{(r-1)}\right),
\quad j=1,\ldots,k.
$$

Each update preserves the target joint law: integrating the old coordinate against its conditional [probability density function](../../../../../../probability-density-function.md) and replacing it by an [independent](../../../../../../independent-random-variables.md) draw from that same conditional leaves the joint [probability density function](../../../../../../probability-density-function.md) unchanged. The composition of the coordinate updates therefore also preserves $\pi$. A [Gibbs sampler](../../../../../../gibbs-sampler.md) coordinate move can be regarded as a [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) move with acceptance [probability](../../../../../../probability.md) one. Systematic sweeps preserve [stationarity](../../../../../../stationary-process.md) but need not themselves be reversible. Initialization away from [stationarity](../../../../../../stationary-process.md) requires convergence before treating the draws as approximately target-distributed, and dependence must be accounted for in [Monte Carlo method](../../../../../../monte-carlo-method.md) error estimates.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
