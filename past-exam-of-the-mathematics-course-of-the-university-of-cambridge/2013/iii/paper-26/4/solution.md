<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Independent [bond percolation](../../../../../bond-percolation-split.md) turns a deterministic [graph](../../../../../graph-split.md) into a random network: each [edge](../../../../../edge-of-a-graph.md) is open with probability $p$, independently, and a [percolation cluster](../../../../../percolation-cluster.md) is a [connected component](../../../../../connected-component.md) of its open subgraph. [Site percolation](../../../../../site-percolation-split.md) instead randomizes vertices. On the [cubic lattice](../../../../../cubic-lattice.md) the [percolation probability](../../../../../percolation-probability.md) $\theta(p)=P_p(0\leftrightarrow\infty)$ is the order parameter and $p_c=\inf\{p:\theta(p)>0\}$ is the [critical probability](../../../../../percolation-critical-probability.md). A monotone coupling, using independent uniform [edge](../../../../../edge-of-a-graph.md) labels and opening labels below $p$, makes the growth of connectivity with $p$ transparent.

For $d\geq2$, $0<p_c<1$: [self-avoiding walk](../../../../../self-avoiding-walk.md) counting gives $p_c\geq1/\mu(d)$, and the planar bound proved above gives an upper bound below one. Below $p_c$, clusters are finite and connection probabilities decay exponentially, a [percolation sharpness theorem](../../../../../sharpness-of-the-percolation-transition.md) rather than a consequence of the threshold definition alone. Above $p_c$ there is almost surely a unique [infinite percolation cluster](../../../../../infinite-percolation-cluster.md). At criticality, the presence of an [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) must be addressed for the particular model. In two dimensions there is none. The transition replaces a finite characteristic length by scale-free geometry, followed by a macroscopic [connected component](../../../../../connected-component.md).

[Percolation critical exponents](../../../../../percolation-critical-exponents.md) quantify different aspects of this change. Use power-law notation for leading exponents; it may suppress amplitudes and logarithmic corrections. From the subcritical side, define the [percolation susceptibility](../../../../../percolation-susceptibility.md) $\chi(p)=\mathbb E_p|C(0)|$ and an exponential [correlation length](../../../../../correlation-length.md) $\xi(p)=1/\lambda(p)$, using a fixed norm for the one-arm rate. Above criticality the unrestricted expectation is infinite, so a finite-cluster [percolation susceptibility](../../../../../percolation-susceptibility.md) must exclude the [infinite percolation cluster](../../../../../infinite-percolation-cluster.md). The principal observables are:

| Exponent | Observable and convention | $\beta$ | $\theta(p)=(p-p_c)^{\beta+o(1)}$ from above | $\gamma$ | $\chi(p)=(p_c-p)^{-\gamma+o(1)}$ from below | $\nu$ | $\xi(p)=|p-p_c|^{-\nu+o(1)}$ for a finite-cluster [correlation length](../../../../../correlation-length.md) | $\delta$ | $P_{p_c}(|C(0)|\geq s)=s^{-1/\delta+o(1)}$ | $\eta$ | Critical two-point connectivity has leading power $|x|^{-(d-2+\eta)}$ | $\tau$ | The expected number per lattice site of size-$s$ clusters has leading power $s^{-\tau}$ |
| --- | --- | --- | --- | --- | --- | --- |

The last distribution is not the distribution seen from a uniformly chosen site: the latter is weighted by cluster size. In the scaling description this accounts for $1/\delta=\tau-2$. Under the usual below-upper-critical-dimension scaling hypotheses, further [scaling relations for critical exponents](../../../../../scaling-relation-for-critical-exponents.md) include

$$
\gamma=(2-\eta)\nu,\qquad\beta\delta=\beta+\gamma,\qquad2\beta+\gamma=d\nu.
$$

They organize the exponents into a small number of independent quantities; they are not automatic identities following only from their definitions. A [percolation cluster fractal dimension](../../../../../percolation-cluster-fractal-dimension.md) $D_f$ describes the mass of a large critical cluster of radius $r$ as roughly $r^{D_f}$, with the [scaling relation for critical exponents](../../../../../scaling-relation-for-critical-exponents.md) $D_f=d-\beta/\nu$ in this regime.

The [percolation universality hypothesis](../../../../../percolation-universality-hypothesis.md) is that ordinary short-range independent models in the same spatial dimension share these exponents and their continuum behavior despite differing microscopic lattices or using bonds rather than sites. The threshold itself is not universal. Long-range connections, correlations or changes of geometry can change the [universality class](../../../../../universality-class.md), so the hypothesis does not include every random [graph](../../../../../graph-split.md) called percolation.

Two dimensions have a particularly strong geometric structure. Closed [planar dual graph](../../../../../planar-dual-graph.md) circuits obstruct primal open paths. The [Harris-Kesten theorem](../../../../../harris-kesten-theorem.md) fixes the [square lattice](../../../../../square-lattice.md) [bond percolation](../../../../../bond-percolation-split.md) threshold at $p_c=1/2$, using planar duality and crossing estimates. Self-duality alone is not a proof; uniform rectangle-crossing control is a crucial extra ingredient. The [Russo-Seymour-Welsh theorem](../../../../../russo-seymour-welsh-theorem.md) keeps critical crossing probabilities of rectangles of fixed aspect ratio bounded away from zero and one at all scales. Closed dual circuits on disjoint annular scales then rule out an infinite critical cluster and reveal why arbitrarily large finite structures persist.

Critical [site percolation](../../../../../site-percolation-split.md) on the [triangular lattice](../../../../../triangular-lattice.md) has rigorously established [conformal invariance of planar percolation](../../../../../conformal-invariance-of-planar-percolation.md) for crossing limits and an [SLE](../../../../../schramm-loewner-evolution.md) description of interfaces. These results are specific to this model. The exact planar values

$$
\boxed{\beta=\frac5{36},\qquad\gamma=\frac{43}{18},\qquad\nu=\frac43}
$$

are rigorously established there; its [one-arm probability](../../../../../one-arm-probability.md) has exponent $5/48$. In the corresponding scaling description these values give $\eta=5/24$, $\delta=91/5$, $\tau=187/91$ and $D_f=91/48$. The [percolation universality hypothesis](../../../../../percolation-universality-hypothesis.md) predicts the same planar exponents for [square lattice](../../../../../square-lattice.md) [bond percolation](../../../../../bond-percolation-split.md), but the triangular-lattice theorem by itself does not prove that transfer. This distinction separates exact model-specific mathematics from a broader physical prediction.

Dimension changes the importance of loops and correlations between growing branches. The [mean-field percolation exponents](../../../../../mean-field-percolation-exponents.md) come from approximating critical clusters by [branching processes](../../../../../branching-process.md). Their values are $\beta=1$, $\gamma=1$, $\delta=2$, $\nu=1/2$, $\eta=0$ and $\tau=5/2$. The predicted [upper critical dimension of percolation](../../../../../upper-critical-dimension-of-percolation.md) is six. One way to see its role is the triangle diagram appearing in the [percolation triangle condition](../../../../../percolation-triangle-condition.md): if the long-distance Fourier connectivity behaves like $|k|^{-2}$, its infrared contribution is proportional to $\int_0^\varepsilon r^{d-7}\,dr$. It is finite above six and logarithmically divergent at six. This motivates mean-field behavior above six and logarithmic corrections at six, without turning that heuristic into a proof for every lattice.

[Lace expansion](../../../../../lace-expansion.md) makes the mean-field picture rigorous in suitable high-dimensional regimes. For nearest-neighbor percolation, sufficiently high dimensions are covered; sufficiently spread-out models have mean-field results for every $d>6$. Between two and six the exponents depend nontrivially on dimension, and exact three-dimensional values are not supplied by the planar theory. [Hyperscaling relation](../../../../../hyperscaling-relation.md) illustrates the change: mean-field values give $2\beta+\gamma=3$, while $d\nu=d/2$, so the naive equality fails above six. In $d=1$, $p_c=1$ and no [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) exists for $p<1$; this is a degenerate endpoint case rather than the ordinary interior transition.

**The threshold locates the transition, [critical exponents](../../../../../critical-exponent.md) describe its geometry and singularities, and the [percolation universality hypothesis](../../../../../percolation-universality-hypothesis.md) proposes which microscopic distinctions disappear at large scales. [Planar dual graph](../../../../../planar-dual-graph.md) arguments and [conformal invariance of planar percolation](../../../../../conformal-invariance-of-planar-percolation.md) make $d=2$ exceptional, while six marks the expected boundary of mean-field scaling.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
