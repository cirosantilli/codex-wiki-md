<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In [bond percolation](../../../../../bond-percolation-split.md) on $\mathbb Z^d$, [edges](../../../../../edge-of-a-graph.md) are independently open with [probability](../../../../../probability.md) $p$ and closed otherwise. An open [percolation cluster](../../../../../percolation-cluster.md) is a connected component using only open [edges](../../../../../edge-of-a-graph.md). In [site percolation](../../../../../site-percolation-split.md) it is the [graph vertices](../../../../../vertex-graph-theory.md) that are independently declared open. The [percolation probability](../../../../../percolation-probability.md) $\theta(p)=P_p(0\leftrightarrow\infty)$ measures the chance that the origin lies in an [infinite percolation cluster](../../../../../infinite-percolation-cluster.md), and the [percolation critical probability](../../../../../percolation-critical-probability.md) is $p_c=\inf\{p:\theta(p)>0\}$. [Monotone coupling of Bernoulli percolation](../../../../../monotone-coupling-of-bernoulli-percolation.md) by independent [uniform distribution](../../../../../continuous-uniform-distribution.md) makes $\theta$ nondecreasing.

The [sharpness of the percolation transition](../../../../../sharpness-of-the-percolation-transition.md) says that below $p_c$ connection [probabilities](../../../../../probability.md) on $\mathbb Z^d$ decay exponentially with distance, while above $p_c$ the percolation [probability](../../../../../probability.md) is positive. There is almost surely a unique [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) in the supercritical regime. On the [square lattice](../../../../../square-lattice.md), the [Harris-Kesten theorem](../../../../../harris-kesten-theorem.md) gives bond threshold $1/2$, and there is no [infinite percolation cluster](../../../../../infinite-percolation-cluster.md) at [percolation critical probability](../../../../../percolation-critical-probability.md). The emergence of connections on arbitrarily large scales is the geometric meaning of the [phase transition](../../../../../phase-transition.md).

Several observables describe this singular behavior. The [percolation susceptibility](../../../../../percolation-susceptibility.md) is $\chi(p)=E_p|C(0)|$ for $p<p_c$. A directional [correlation length](../../../../../correlation-length.md) can be defined through exponential two-point decay, $\xi(p)^{-1}=-\lim_n n^{-1}\log P_p(0\leftrightarrow ne_1)$. [Percolation critical exponents](../../../../../percolation-critical-exponents.md) describe leading powers, conveniently defined logarithmically rather than requiring exact asymptotic amplitudes:

$$
\theta(p)=(p-p_c)^{\beta+o(1)},\quad
\chi(p)=(p_c-p)^{-\gamma+o(1)},\quad
\xi(p)=(p_c-p)^{-\nu+o(1)}.
$$

The first [limit of a sequence](../../../../../limit-of-a-sequence.md) approaches from above, the other two from below. At [percolation critical probability](../../../../../percolation-critical-probability.md), [percolation two-point connection probability](../../../../../percolation-two-point-connection-probability.md) is expected to have leading power $|x|^{-(d-2+\eta)}$, and the number per site of [percolation clusters](../../../../../percolation-cluster.md) of size $s$ has leading power $s^{-\tau}$. This cluster-count [probability distribution](../../../../../probability-distribution.md) differs from the size-biased [probability distribution](../../../../../probability-distribution.md) seen by choosing a site. [Scaling relations for critical exponents](../../../../../scaling-relation-for-critical-exponents.md) such as $\gamma=(2-\eta)\nu$ and $2\beta+\gamma=d\nu$ connect the exponents in their applicable scaling regime; [hyperscaling relation](../../../../../hyperscaling-relation.md) is not valid above the [upper critical dimension of percolation](../../../../../upper-critical-dimension-of-percolation.md) in ordinary mean-field regimes.

The [percolation universality hypothesis](../../../../../percolation-universality-hypothesis.md) predicts that dimension and large-scale symmetry, rather than microscopic [graph](../../../../../graph-split.md) details, determine these exponents and scaling functions. Thus square-lattice bond and triangular-lattice site models are expected to share the [planar graph](../../../../../planar-graph.md) [universality class](../../../../../universality-class.md) despite different microscopic definitions. Universality does not mean identical critical [probabilities](../../../../../probability.md), amplitudes or finite-lattice distributions. Exact values and existence of exponents require model-specific theorems, not merely this prediction.

Two dimensions have an additional structure: [conformal maps](../../../../../conformal-map.md) preserve angles, and critical crossing [probabilities](../../../../../probability.md) are expected to be unchanged under conformal transport of the domain and its marked boundary arcs. A crossing [probability](../../../../../probability.md) then depends only on the conformal shape of that marked quadrilateral. The [Cardy boundary crossing formula](../../../../../cardy-boundary-crossing-formula.md) gives this dependence in terms of its boundary cross ratio. For critical triangular-lattice site percolation, conformal invariance and the resulting exponents are established; examples are $\beta=5/36$, $\gamma=43/18$, $\nu=4/3$, with the rigorous statements in leading-power form. These values are summarized in [Smirnov and Werner's original paper](https://www.unige.ch/~smirnov/papers/smw-j.pdf). Their universality extension to arbitrary planar lattices should not be presented as the same theorem.

An exploration path separating the two colors, with opposite boundary colors on two arcs, has a [domain Markov property of a percolation exploration](../../../../../domain-markov-property-of-a-percolation-exploration.md): conditional on the explored portion, the unexplored colors retain their independent laws with the newly exposed boundary colors. Conformal invariance, this domain Markov property and suitable regularity lead to [Schramm–Loewner evolution](../../../../../schramm-loewner-evolution.md). In the upper half-plane its chordal equation is

$$
\partial_tg_t(z)=\frac2{g_t(z)-U_t},\qquad U_t=\sqrt\kappa\,B_t,
$$

where $B_t$ is standard [Brownian motion](../../../../../brownian-motion-split.md) and time is normalized by half-plane capacity. Critical percolation corresponds to $\kappa=6$. Thus the complicated discrete interface becomes a conformally natural random curve driven by one real [Brownian motion](../../../../../brownian-motion-split.md). Its crossing and arm [probabilities](../../../../../probability.md) supply critical exponents and, through [scaling relations for critical exponents](../../../../../scaling-relation-for-critical-exponents.md), near-critical singularities. This makes conformal methods predictive tools for the transition, rather than only descriptions of an interface's appearance.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
