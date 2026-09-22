<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the inner boundary specified in the PDF, the [Ising boundary condition](../../../../../../ising-boundary-condition.md) pins $\omega|_{\partial\Lambda}=\zeta$. Explicitly $\mu_\Lambda^\zeta$ is $\mu_\Lambda$ conditioned on those [Ising spins](../../../../../../ising-spin-variable.md). Its [partition function](../../../../../../canonical-partition-function.md) sums over unpinned interior [Ising spins](../../../../../../ising-spin-variable.md) only; [edges](../../../../../../edge-of-a-graph.md) between two pinned sites contribute a constant that cancels on normalization.

Pinning coordinates preserves the [FKG lattice condition](../../../../../../fkg-lattice-condition.md), since [meet in a lattice](../../../../../../meet-in-a-lattice.md) and [join in a lattice](../../../../../../join-in-a-lattice.md) still have the same pinned values. It also gives monotonicity in the pins. For any [increasing observable](../../../../../../increasing-function-on-a-partially-ordered-set.md) $f$, [positive association of random variables](../../../../../../positive-association-of-random-variables.md) with an unpinned [Ising spin](../../../../../../ising-spin-variable.md) $\omega(z)$ gives

$$
E[f\mid\omega(z)=1]\ge E[f\mid\omega(z)=0].
$$

Both [conditional probabilities](../../../../../../conditional-probability.md) are positive. The same inequality holds after other [Ising spins](../../../../../../ising-spin-variable.md) have been pinned. Changing pins one at a time proves [stochastic domination](../../../../../../stochastic-domination-of-probability-measures.md) of the measures as $\zeta$ increases.

Now let $\Lambda\subset\Lambda'$ and take an [increasing observable](../../../../../../increasing-function-on-a-partially-ordered-set.md) depending on a fixed set inside the smaller box. Given the [Ising spins](../../../../../../ising-spin-variable.md) on $\partial\Lambda$, the larger-box measure induces precisely the smaller-box interior law with those boundary values: nearest-neighbor interactions cannot see farther once this boundary is fixed. Its conditional law is therefore between the all-zero and all-one smaller-box laws. Averaging yields

$$
\mu_\Lambda^0(f)\le\mu_{\Lambda'}^0(f),\qquad
\mu_{\Lambda'}^1(f)\le\mu_\Lambda^1(f).
$$

These are bounded monotone sequences along any increasing box exhaustion.

For every finite set $S$, the event that all [Ising spins](../../../../../../ising-spin-variable.md) in $S$ are one is increasing, so its [probability](../../../../../../probability.md) converges in both boundary sequences. [Probabilities](../../../../../../probability.md) of arbitrary finite zero/one patterns are finite [inclusion-exclusion](../../../../../../inclusion-exclusion-principle.md) combinations of these all-one [probabilities](../../../../../../probability.md), and hence converge too. The limits are consistent [finite-dimensional distributions](../../../../../../finite-dimensional-distribution.md); they define measures on $\{0,1\}^{\mathbb Z^d}$ and give [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md) in the [product topology](../../../../../../product-topology.md). Thus **both [extremal infinite-volume Ising measures](../../../../../../extremal-infinite-volume-ising-measures.md) $\mu^0,\mu^1$ exist**, with $\mu^0$ below $\mu^1$ in [stochastic domination](../../../../../../stochastic-domination-of-probability-measures.md). This argument proves existence even when the two limits are different.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
