<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A clean proof outline uses [hypergraph removal](../../../../../hypergraph-removal.md) rather than the quadratic [density increment](../../../../../density-increment.md) route. The structure is: establish removal for the [three-uniform tetrahedron](../../../../../three-uniform-tetrahedron.md), encode four-term [arithmetic progressions](../../../../../arithmetic-progression.md) as its copies, and use the many edge-disjoint copies coming from constant progressions to contradict removal. We give the technical regularity stage in outline, as requested, and prove the counting inequality and the encoding that make the argument work.

The needed [tetrahedron removal lemma](../../../../../tetrahedron-removal-lemma.md) says that for each $\eta>0$ there is $\rho>0$ such that a three-[uniform hypergraph](../../../../../uniform-hypergraph.md) on $v$ vertices with fewer than $\rho v^4$ copies of $K_4^3$ can be made $K_4^3$-free by removing fewer than $\eta v^3$ hyperedges. Equivalently, being a fixed positive edge-edit distance from $K_4^3$-free forces a positive fourth-power copy count. Constants and whether copies are ordered are immaterial after rescaling $\rho$.

Here is the global proof of this [hypergraph removal](../../../../../hypergraph-removal.md) input. [Strong regularity for three-uniform hypergraphs](../../../../../strong-regularity-for-three-uniform-hypergraphs.md) partitions both vertices and the bipartite pair sets between vertex classes. The resulting three-class cells, called [triads in a hypergraph regularity partition](../../../../../triad-in-a-hypergraph-regularity-partition.md), are supported on three pair cells. On all but a prescribed small total weight, the triple-edge function has approximately constant relative density and a small relative three-dimensional [box norm](../../../../../box-norm.md). This two-level refinement is essential: a vertex partition alone does not capture correlations carried by pairs. The regularity construction uses the squared [L2 norms](../../../../../l2-norm.md) of [conditional expectations](../../../../../conditional-expectation.md) of edge indicators as bounded energies. Refinement increases this energy by the squared [L2 norm](../../../../../l2-norm.md) of the difference between the new and old [conditional expectations](../../../../../conditional-expectation.md), by orthogonality. Thus a nonuniformity witness causing a definite discrepancy causes a definite energy increment. A witness to nonuniformity refines the relevant pair or triple partition and raises the appropriate energy. A hierarchy of tolerances, with sufficiently strong refinement at the pair level, makes these increases terminate after a bounded number of stages. Bounds may depend very badly on the requested tolerance, which is harmless for a qualitative theorem.

Delete hyperedges with two vertices in the same vertex class, hyperedges meeting exceptional classes or irregular cells, hyperedges supported on pair cells of very small density, and hyperedges in triads of very small triple density. Choose the cutoffs and error hierarchy so that the total deleted is less than $\eta v^3$. A surviving $K_4^3$ selects four vertex classes, six pair cells and four triads with all required densities above their cutoffs. The relative [tetrahedron counting lemma](../../../../../tetrahedron-counting-lemma.md) gives at least $\rho v^4$ copies in those cells. This contradicts the assumed sparse copy count, and proves the [tetrahedron removal lemma](../../../../../tetrahedron-removal-lemma.md). The strong regularity and relative counting estimates are the technical portion outlined here; the dependence of their constants is not needed.

To show the key analytic mechanism in that counting step, define the [three-dimensional box norm](../../../../../three-dimensional-box-norm.md) of a complex function on $X_1\times X_2\times X_3$ by

$$
\|g\|_{\square^3}^8=\mathbb E_{x_j^0,x_j^1}
\prod_{\omega\in\{0,1\}^3}\mathcal C^{|\omega|}g(x_1^{\omega_1},x_2^{\omega_2},x_3^{\omega_3}),
$$

where $\mathcal C$ denotes complex conjugation. If the other three functions are bounded by one, then

$$
\left|\mathbb E_{x_0,x_1,x_2,x_3}
 g(x_1,x_2,x_3)g_1(x_0,x_2,x_3)g_2(x_0,x_1,x_3)g_3(x_0,x_1,x_2)\right|
\leq\|g\|_{\square^3}.
$$

For a proof, fix $x_0$ first. Apply the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) over $(x_2,x_3)$ to remove $g_1$, duplicating $x_1$. Next apply the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) over the variables other than $x_2$ to remove the two factors from $g_2$, duplicating $x_2$. A third application removes the four factors from $g_3$ and duplicates $x_3$. The resulting eighth power is exactly the cube average displayed above. Averaging over $x_0$ proves the inequality. This also shows nonnegativity of the cube average by its successive squared-sum form.

For example, on complete pair supports, if four triple-edge functions $f_i$ have constant parts $d_i$ and $\|f_i-d_i\|_{\square^3}\leq\xi$, telescope the fourfold product and apply this inequality to each term. Their [hypergraph clique](../../../../../complete-uniform-hypergraph.md) density differs from $d_0d_1d_2d_3$ by at most $4\xi$, so it is positive when $4\xi<\prod_i d_i$. On general pair supports the same successive squaring argument is combined with sufficiently regular pair cells; choosing relative errors small compared with the pair-density product gives the relative [tetrahedron counting lemma](../../../../../tetrahedron-counting-lemma.md). This explains both the counting step and why its support must be regularized before the triple-edge densities. It supplies a proved important step without pretending that the strong regularity theorem is a one-line assertion.

We now prove the [four-term progression hypergraph encoding](../../../../../four-term-progression-hypergraph-encoding.md) completely. Let $A\subseteq[N]$ have [subset density](../../../../../density-of-a-finite-subset.md) at least $\delta>0$, choose $M=4N+1$, and take four disjoint copies $X_0,\ldots,X_3$ of the [cyclic group](../../../../../cyclic-group.md) $G=\mathbb Z/M\mathbb Z$. Put a hyperedge on the three vertices excluding part $i$ precisely when

$$
L_i((x_j)_{j\ne i})=\sum_{j\ne i}(j-i)x_j\in A.
$$

For a transversal quadruple let $S_0=\sum_jx_j$ and $S_1=\sum_jjx_j$. Its four edge conditions are $S_1-iS_0\in A$, $i=0,1,2,3$. Thus a $K_4^3$ gives a four-term [arithmetic progression](../../../../../arithmetic-progression.md) with common difference $-S_0$ modulo $M$.

Suppose $A$ has no nonconstant four-term [arithmetic progression](../../../../../arithmetic-progression.md) in the [integers](../../../../../integer.md). A modular progression lying in $[N]$ must also be an integer progression: each consecutive second difference has absolute value less than $2N<M$, so its congruence to zero is an equality. Therefore every $K_4^3$ in this [hypergraph](../../../../../hypergraph-split.md) has $S_0=0$, and all four values equal some $a\in A$. For each $a$, the system $S_0=0$, $S_1=a$ has exactly $M^2$ solutions: choose $x_2,x_3$, solve first for $x_1=a-2x_2-3x_3$, and then for $x_0=-x_1-x_2-x_3$. There are exactly $|A|M^2=O(M^3)$ copies of $K_4^3$.

These copies are edge-disjoint. Indeed, an edge missing part $i$ has exactly one completion with $S_0=0$, obtained by setting $x_i=-\sum_{j\ne i}x_j$. Its common value is the already prescribed $L_i\in A$. Hence destroying all copies requires at least $|A|M^2$ edge deletions. Since $M\leq5N$, this is at least $\delta M^3/5$. Apply the [tetrahedron removal lemma](../../../../../tetrahedron-removal-lemma.md) to the $v=4M$ vertices with, for instance, $\eta=\delta/640$. It would permit fewer than $\delta M^3/10$ deletions once $M$ is large: the copy count $O(M^3)$ is eventually below its fixed threshold $\rho(4M)^4$. This is impossible.

**Every fixed positive density therefore forces a nonconstant four-term arithmetic progression in sufficiently long intervals.** This proves the length-four case of the [Szemerédi theorem](../../../../../szemeredi-s-theorem.md). Applying it to sufficiently large initial intervals along a subsequence witnessing positive [upper asymptotic density](../../../../../upper-asymptotic-density.md) also gives the usual infinite-set formulation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
