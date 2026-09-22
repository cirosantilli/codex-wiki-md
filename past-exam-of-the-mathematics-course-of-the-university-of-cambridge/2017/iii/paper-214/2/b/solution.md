<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use [planar duality for rectangle crossings](../../../../../../planar-duality-for-rectangle-crossings.md), [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) and the permitted [exponential decay of subcritical percolation](../../../../../../exponential-decay-of-subcritical-percolation.md). A critical-point detail matters: uniqueness stated only for $p>p_c$ cannot by itself be applied at $p=p_c$. We prove the [Burton-Keane theorem](../../../../../../uniqueness-of-the-infinite-percolation-cluster.md) by the [boundary counting proof of percolation uniqueness](../../../../../../boundary-counting-proof-of-percolation-uniqueness.md), establishing at most one [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) at every parameter and avoiding that gap.

For $0<p<1$, the number $N$ of [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) is [almost surely](../../../../../../almost-sure-convergence.md) constant by [translation ergodicity of Bernoulli percolation](../../../../../../translation-ergodicity-of-bernoulli-percolation.md). It cannot be a finite constant greater than one. A sufficiently large box meets two different [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) with positive [probability](../../../../../../probability.md); opening its finitely many interior [edges](../../../../../../edge-of-a-graph.md) joins them without creating a new [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md), decreasing $N$. [Finite modification of Bernoulli percolation](../../../../../../finite-modification-of-bernoulli-percolation.md) gives positive [probability](../../../../../../probability.md) to this modification, contradicting constancy.

Nor can $N=\infty$. A finite box then meets three different [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) with positive [probability](../../../../../../probability.md). Select one infinite exterior branch from each. In the box and a finite collar retain just an embedded three-armed [tree](../../../../../../tree-graph-theory.md) joining those branches and close all other incident [edges](../../../../../../edge-of-a-graph.md) there. Its branching [graph vertex](../../../../../../vertex-graph-theory.md) separates three infinite components when removed, so is a [trifurcation vertex in percolation](../../../../../../trifurcation-vertex-in-percolation.md). All selections concern finitely many possible entrances and [edge](../../../../../../edge-of-a-graph.md) patterns; [finite-energy property of Bernoulli percolation](../../../../../../finite-energy-property-of-bernoulli-percolation.md) gives positive [probability](../../../../../../probability.md) for at least one such pattern. Translation invariance then gives a common positive trifurcation [probability](../../../../../../probability.md) $q$.

Here is the counting contradiction in detail. For a finite box $W$, contract each open component outside $W$ that touches $W$ to a boundary terminal. In each cluster, the resulting incidence [graph](../../../../../../graph-split.md) is finite and connected. Every trifurcation in $W$ separates at least three sets of terminals, since each infinite branch must leave $W$. A minimal subtree joining all terminals must therefore contain that [graph vertex](../../../../../../vertex-graph-theory.md) with [degree of a vertex](../../../../../../degree-graph-theory.md) at least three. Its leaves are terminals. The [tree](../../../../../../tree-graph-theory.md) identity $\sum_v(\deg(v)-2)=-2$ bounds the number of those branching [graph vertices](../../../../../../vertex-graph-theory.md) by the terminal count. Different terminals are represented by different exterior [graph neighbours](../../../../../../neighbour-of-a-vertex.md) of $W$. Thus the [trifurcation boundary-counting lemma](../../../../../../trifurcation-boundary-counting-lemma.md) gives

$$
q|W|=\mathbb E\bigl[\#\{v\in W:v\text{ trifurcates}\}\bigr]\leq|\partial^+W|.
$$

For $W=[-r,r]^2\cap\mathbb Z^2$, the two sizes are $(2r+1)^2$ and $8r+4$. Letting $r\to\infty$ contradicts $q>0$. Therefore $N\in\{0,1\}$ [almost surely](../../../../../../almost-sure-convergence.md), with the same conclusion for the translated [planar dual graph](../../../../../../planar-dual-graph.md).

Now prove absence of percolation at $p=1/2$ by [Zhang's argument](../../../../../../alternating-arms-argument-at-the-self-dual-percolation-parameter.md). Suppose instead that $\theta(1/2)>0$. [Almost surely](../../../../../../almost-sure-convergence.md) an infinite primal cluster exists, and self-duality gives an infinite dual cluster as well. An infinite connected subgraph of this locally finite lattice contains a [graph ray](../../../../../../ray-in-a-graph.md), by the [König infinity lemma](../../../../../../konig-s-lemma.md). Expanding square boxes meet the [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md) with [probability](../../../../../../probability.md) tending to one.

For $B_r=[-r,r]^2\cap\mathbb Z^2$, let $A_N,A_E,A_S,A_W$ mean that an open [graph ray](../../../../../../ray-in-a-graph.md) takes an outward [edge](../../../../../../edge-of-a-graph.md) through the indicated side and subsequently uses [graph vertices](../../../../../../vertex-graph-theory.md) outside $B_r$. The union occurs whenever the box meets an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md): take the last exit of an infinite [graph ray](../../../../../../ray-in-a-graph.md) from the finite box. Conversely an exterior arm supplies an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) meeting its boundary. Quarter-turn symmetry makes the four [probabilities](../../../../../../probability.md) equal. Their complements are [decreasing events](../../../../../../decreasing-event.md), so the [square-root trick for positively associated events](../../../../../../square-root-trick-for-positively-associated-events.md) gives

$$
\mathbb P_{1/2}(A_N)\geq1-\mathbb P_{1/2}(B_r\not\leftrightarrow\infty)^{1/4}\longrightarrow1.
$$

For the [planar dual graph](../../../../../../planar-dual-graph.md) use the box with boundary coordinates $\pm(r+1/2)$ and define its exterior side-arm events in the same way. This box also has quarter-turn symmetry and meets the dual [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) with [probability](../../../../../../probability.md) tending to one. Thus each dual side has an infinite exterior arm with [probability](../../../../../../probability.md) tending to one. Primal outward [edges](../../../../../../edge-of-a-graph.md) cross this dual-box contour on the corresponding sides; their remaining [graph vertices](../../../../../../vertex-graph-theory.md) stay outside it. A [union bound](../../../../../../boole-s-inequality.md) makes the simultaneous event of primal north/south arms and dual east/west arms have positive [probability](../../../../../../probability.md) for a sufficiently large box.

The four arms alternate around the contour. Open all [edges](../../../../../../edge-of-a-graph.md) with both endpoints in $B_r$, leaving all outward and exterior [edges](../../../../../../edge-of-a-graph.md) intact. This joins the two primal entrance points and preserves all four exterior arms. [Finite-energy property of Bernoulli percolation](../../../../../../finite-energy-property-of-bernoulli-percolation.md) keeps the event's [probability](../../../../../../probability.md) positive. The primal north and south arms are now connected through the box. The two dual arms must lie in different infinite dual clusters. To see the separation, a hypothetical finite dual [graph path](../../../../../../path-in-a-graph.md) joining the east and west arms cannot enter the dual-box interior: its boundary-crossing and interior [edges](../../../../../../edge-of-a-graph.md) cross primal [edges](../../../../../../edge-of-a-graph.md) that were just opened. Erase its loops and cut it at successive hits of the contour. A resulting exterior dual crosscut, together with the corresponding contour arc, encloses one of the two intervening primal entrance points. The infinite primal [graph ray](../../../../../../ray-in-a-graph.md) from that point would have to cross a dual-open [edge](../../../../../../edge-of-a-graph.md), which is impossible. This is the planar separation used in the [alternating arms argument at the self-dual percolation parameter](../../../../../../alternating-arms-argument-at-the-self-dual-percolation-parameter.md). It contradicts uniqueness of the infinite dual cluster. Hence

$$
\boxed{\theta(1/2)=0,\qquad p_c(2)\geq1/2.}
$$

Finally suppose $p_c(2)>1/2$. At $p=1/2$ the permitted [exponential decay of subcritical percolation](../../../../../../exponential-decay-of-subcritical-percolation.md) would supply $C,c>0$ with $\mathbb P_{1/2}(v\leftrightarrow\partial B_n(v))\leq Ce^{-cn}$. Use the rectangle with [graph vertices](../../../../../../vertex-graph-theory.md) $\{0,\ldots,n\}\times\{0,\ldots,n-1\}$, and let $H_n$ be its left-to-right open crossing. [Planar duality for rectangle crossings](../../../../../../planar-duality-for-rectangle-crossings.md) identifies its complement with a dual top-to-bottom crossing of a rectangle of width $n-1$ and height $n$. Rotation and translation give the same crossing law; side [edges](../../../../../../edge-of-a-graph.md) at the entrance and exit boundaries are irrelevant. Thus the [exact self-dual rectangle crossing probability](../../../../../../exact-self-dual-rectangle-crossing-probability.md) is

$$
\mathbb P_{1/2}(H_n)=\frac12.
$$

But a crossing has some starting [graph vertex](../../../../../../vertex-graph-theory.md) on its $n$-vertex left side connected to distance $n$. The [union bound](../../../../../../boole-s-inequality.md) and [exponential decay of subcritical percolation](../../../../../../exponential-decay-of-subcritical-percolation.md) imply $\mathbb P_{1/2}(H_n)\leq nCe^{-cn}\to0$, a contradiction. Therefore

$$
\boxed{p_c(2)=1/2\quad\text{and}\quad\theta(1/2)=0.}
$$

No Russo-Seymour-Welsh theorem or continuity assertion for $\theta$ is being used, and critical uniqueness was proved rather than inferred from the supercritical hypothesis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
