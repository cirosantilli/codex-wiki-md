<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The duality requested below uses the [symmetric simple exclusion process](../../../../../../symmetric-simple-exclusion-process.md), so we take that standard convention here. A configuration $\eta\in\{0,1\}^{\mathbb Z}$ records a particle at $x$ when $\eta(x)=1$. Particles attempt nearest-neighbour jumps with equal left and right rates, and any attempt into an occupied site is suppressed. Thus there is at most one particle at each site.

A convenient normalization puts independent rate-one Poisson clocks on the unoriented [edges](../../../../../../edge-of-a-graph.md) $\{x,x+1\}$. At an [edge](../../../../../../edge-of-a-graph.md) mark, interchange its two endpoint occupations. If both endpoints have the same occupation, nothing changes; if exactly one is occupied, that particle jumps to the vacant endpoint. The generator on cylinder functions is

$$
\boxed{Lf(\eta)=\sum_{x\in\mathbb Z}\bigl[f(\eta^{x,x+1})-f(\eta)\bigr].}
$$

Only finitely many terms can be nonzero for a cylinder function. A convention with total jump-attempt rate one per particle uses [edge](../../../../../../edge-of-a-graph.md) clocks of rate $1/2$, merely rescaling time.

For a pathwise construction, label all sites and swap their labels at each clock mark, carrying the initial occupations along with the labels. Each label path has jump rate two and is nonexplosive on a bounded time interval. The same is true of a backward path from any fixed space-time point. This [stirring representation of symmetric exclusion](../../../../../../stirring-representation-of-symmetric-exclusion.md) therefore defines the occupations for every initial configuration, even with infinitely many particles. It also conserves the number of particles when finite.

A general [exclusion process](../../../../../../exclusion-process.md) may have asymmetric jump rates, but then the plain occupation-product self-duality in the next part need not hold. The symmetry convention is therefore mathematically necessary here, rather than an irrelevant choice of time normalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
