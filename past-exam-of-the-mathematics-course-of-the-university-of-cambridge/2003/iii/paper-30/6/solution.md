<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In the [voter model](../../../../../voter-model.md) on $\mathbb Z^2$, each site has a rate-one [Poisson process](../../../../../poisson-process.md) clock; when it rings, that site copies one of its four neighbors, chosen uniformly. States are zero or one. For a [cylinder function](../../../../../cylinder-function-on-a-product-space.md) $f$, the local [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) is

$$
Lf(\eta)=\sum_x\frac14\sum_{y\sim x}\bigl[f(\eta^{x\leftarrow y})-f(\eta)\bigr],
$$

where $\eta^{x\leftarrow y}$ agrees with $\eta$ except that the [voter model](../../../../../voter-model.md) opinion at $x$ is replaced by the [voter model](../../../../../voter-model.md) opinion at $y$. Only sites in the support of $f$ contribute, so this [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) sum is finite.

The [voter-model duality](../../../../../voter-model-duality.md) comes from independent [Poisson processes](../../../../../poisson-process.md) of copying arrows of rate $1/4$ on each ordered neighboring pair. Trace the ancestors of specified sites backwards from time $t$: each ancestral line is a rate-one [continuous-time random walk](../../../../../continuous-time-random-walk.md) with uniform nearest-neighbor steps, and lines coalesce when they meet. The [voter model](../../../../../voter-model.md) opinions at time $t$ are the initial [voter model](../../../../../voter-model.md) opinions at those ancestral locations. This construction also explains the general duality theorem being used.

Two ancestral walks on $\mathbb Z^2$ meet almost surely. Until their meeting, their difference is a rate-two symmetric nearest-neighbor walk, and [simple random walk in two dimensions is recurrent](../../../../../simple-random-walk-in-two-dimensions-is-recurrent.md). If $\tau_{xy}$ is their meeting time, this gives

$$
P_\nu(\xi_t(x)\ne\xi_t(y))\le P(\tau_{xy}>t)\longrightarrow0
$$

for every initial law $\nu$. If $\nu$ is invariant, the left side is the fixed [probability](../../../../../probability.md) $\nu(\eta(x)\ne\eta(y))$, so it is zero. This holds for every pair. Countability then implies that $\nu$ is concentrated on configurations with all [voter model](../../../../../voter-model.md) opinions equal. Both constant configurations are [absorbing state](../../../../../absorbing-state.md). Thus the [invariant measures of the two-dimensional voter model](../../../../../invariant-measures-of-the-two-dimensional-voter-model.md) are exactly

$$
\boxed{\nu=\alpha\delta_0+(1-\alpha)\delta_1,\qquad0\le\alpha\le1.}
$$

No translation-invariance assumption on $\nu$ was used.

For the last assertion, let the initial set of one-valued opinions $F$ be finite. Single-line duality gives

$$
P(\xi_t(x)=1)=P_x(X_t\in F)=\sum_{z\in F}p_t(x,z).
$$

Each [transition probability](../../../../../transition-probability.md) tends to zero. One direct verification is the [Fourier transform](../../../../../fourier-transform.md) for the rate-one walk:

$$
p_t(x,z)=\frac1{(2\pi)^2}\int_{[-\pi,\pi]^2}
 e^{-ik\cdot(z-x)}\exp\left[-t\left(1-\tfrac12(\cos k_1+\cos k_2)\right)\right]dk.
$$

The integrand has modulus at most one and tends to zero except at the single point $k=0$; [dominated convergence](../../../../../dominated-convergence-theorem.md) proves the claim. For any finite observation set $K$, the [union bound](../../../../../boole-s-inequality.md) now gives

$$
P(\xi_t\text{ has a one somewhere in }K)
\le\sum_{x\in K}\sum_{z\in F}p_t(x,z)\longrightarrow0.
$$

Therefore every finite [voter model](../../../../../voter-model.md) opinion pattern converges in law to the all-zero pattern. These cylinder distributions determine [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md) in the compact [product topology](../../../../../product-topology.md), proving **finite-seed local extinction in the [voter model](../../../../../voter-model.md)** and

$$
\boxed{\mathcal L(\xi_t)\Longrightarrow\delta_0.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
