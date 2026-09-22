<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [equilibrium oddness theorem](../../../../../../equilibrium-oddness-theorem.md) gives a finite odd number of [Nash equilibria](../../../../../../nash-equilibrium.md) in a finite nondegenerate [bimatrix game](../../../../../../bimatrix-game.md). One way to see the parity is through the endpoint argument underlying the [Lemke-Howson algorithm](../../../../../../lemke-howson-algorithm.md). Add sufficiently large constants to each payoff matrix so all entries are positive; this does not change [best responses](../../../../../../best-response.md). Form the bounded [convex polytopes](../../../../../../convex-polytope.md)

$$
X=\{s\geq0:Q^Ts\leq\mathbf1\},\qquad
Y=\{t\geq0:Pt\leq\mathbf1\}.
$$

Label an $s_i=0$ facet by row label $i$ and a tight $(Q^Ts)_j=1$ facet by column label $n+j$; in $Y$, label a tight $(Pt)_i=1$ facet by $i$ and $t_j=0$ by $n+j$. A completely labelled [vertex of a polytope](../../../../../../vertex-of-a-polytope.md) pair has either both vectors zero, or both nonzero and normalizes to a [Nash equilibrium](../../../../../../nash-equilibrium.md). In the latter case the labels express exactly the equilibrium best-response and zero-probability conditions. Nondegeneracy makes each [vertex of a polytope](../../../../../../vertex-of-a-polytope.md) have exactly $n$ distinct incident labels and each equilibrium correspond to one such pair.

Fix a label to drop and retain all pairs carrying every other label. Include the product-[convex polytope](../../../../../../convex-polytope.md) edges that retain those labels. At a completely labelled pair there is one possible outgoing edge, obtained by dropping the fixed label. At any other retained [vertex of a polytope](../../../../../../vertex-of-a-polytope.md), that label is missing and one other label is duplicated; dropping either copy gives the two incident edges. Thus this finite graph consists of paths and cycles, with its endpoints precisely the completely labelled pairs. A finite graph has an even number of degree-one vertices. Since one endpoint is the artificial zero pair, the number of genuine equilibrium endpoints is odd. This proves the required [equilibrium oddness theorem](../../../../../../equilibrium-oddness-theorem.md) and finiteness, without claiming that every equilibrium is reached from the zero pair on the same path.

For a [symmetric bimatrix game](../../../../../../symmetric-bimatrix-game.md), swapping players maps $(s,t)$ to $(t,s)$. Every nonsymmetric equilibrium lies in a distinct two-element pair; the fixed points of this involution are exactly the [symmetric equilibria](../../../../../../symmetric-equilibrium.md). Removing even-sized pairs from an odd total leaves an odd number of symmetric equilibria. In the present game, two equilibria form the swapped pair and the remaining one is $(x,x)$ with $x=(1/2,0,1/2)$. **There is exactly one symmetric equilibrium**, as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
