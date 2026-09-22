<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [standard simplicial decomposition of a sphere](../../../../../standard-simplicial-decomposition-of-a-sphere.md) $F^n$ is the boundary of the [cross-polytope](../../../../../cross-polytope.md) with vertices $\pm e_1,\ldots,\pm e_{n+1}$, identified radially with $S^n$. A face chooses distinct coordinate indices and one sign for each; it never contains an [antipodal pair](../../../../../antipodal-pair.md).

A [regular antipodal triangulation of a sphere](../../../../../regular-antipodal-triangulation-of-a-sphere.md) is invariant under the [antipodal map](../../../../../antipodal-map.md) and has the nested coordinate equators $S^0\subset S^1\subset\cdots\subset S^{k-1}$ as subcomplexes. In particular each equator separates its sphere into two triangulated [hemispheres](../../../../../hemisphere.md). These conditions are preserved by [barycentric subdivision](../../../../../barycentric-subdivision.md).

For a [simplicial map](../../../../../simplicial-map.md) $f:F\to F^n$, a [positive alternating simplex](../../../../../positive-alternating-simplex.md) of dimension $j$ has distinct image labels

$$
+e_{i_0},-e_{i_1},\ldots,(-1)^je_{i_j},\qquad i_0<\cdots<i_j.
$$

The opposite alternating pattern is negative; all other simplices, including collapsed images, are neutral.

To prove the [antipodal alternating-simplex parity lemma](../../../../../antipodal-alternating-simplex-parity-lemma.md), let $p_j$ count positive $j$-simplices in the equatorial $S^j$. There is exactly one positive vertex in $S^0$, so $p_0=1$. A $j$-simplex has an odd number of positive alternating facets precisely when it is positive or negative alternating. Indeed an alternating sequence has exactly one positive alternating deletion; a nonalternating sequence has either zero or two. For a collapsed image, a positive facet can occur only when exactly one label is repeated; deleting either copy gives two such facets.

Count incidences of positive $(j-1)$-faces with $j$-simplices in one closed [hemisphere](../../../../../hemisphere.md). Interior faces contribute twice and equatorial faces once. The count modulo two is therefore $p_{j-1}$. It is also the number of positive or negative $j$-simplices in that hemisphere modulo two. Because $f$ is antipodal, each alternating pair $\sigma,-\sigma$ has one positive and one negative member, with one member in each hemisphere. Thus

$$
p_j\equiv p_{j-1}\pmod2.
$$

Induction gives odd $p_k$, proving the existence of a positive $k$-simplex. In particular, an antipodal [simplicial map](../../../../../simplicial-map.md) $F\to F^{k-1}$ is impossible: a positive $k$-simplex would require $k+1$ distinct coordinate labels but only $k$ are available.

The [Borsuk-Ulam theorem](../../../../../borsuk-ulam-theorem.md) states that every [continuous map](../../../../../continuous-map.md) $g:S^k\to\mathbb R^k$ has some $x$ with $g(x)=g(-x)$. First rule out a continuous antipodal map $h:S^k\to S^{k-1}$ for $k\geq1$. By [uniform continuity](../../../../../uniform-continuity.md), take a sufficiently fine regular [barycentric subdivision](../../../../../barycentric-subdivision.md) so that endpoints of each edge have images less than $2/\sqrt{k}$ apart. Label a vertex by $\operatorname{sgn}(h_i)e_i$, where $i$ is the smallest index maximizing $|h_i|$. Since $h$ is unit length, this maximum is at least $1/\sqrt{k}$; two adjacent vertices cannot have opposite labels. The labels therefore define an antipodal [simplicial map](../../../../../simplicial-map.md) to $F^{k-1}$, contradicting the preceding result.

If the stated [Borsuk-Ulam theorem](../../../../../borsuk-ulam-theorem.md) failed, the map

$$
h(x)=\frac{g(x)-g(-x)}{\|g(x)-g(-x)\|}
$$

would be just such a continuous antipodal map. This proves the required version; $k=0$ is immediate.

For the [Kneser conjecture](../../../../../lovasz-theorem-on-kneser-graphs.md), equivalently [Lovász theorem on Kneser graphs](../../../../../lovasz-theorem-on-kneser-graphs.md), the claim is

$$
\boxed{\chi(KG(N,r))=N-2r+2\qquad(N\geq2r\geq2)}.
$$

The [Kneser graph](../../../../../kneser-graph.md) joins disjoint $r$-subsets of $[N]$. Let $d=N-2r+1$. Colour each $r$-set by its least element in $[d]$ when it has one, and otherwise by one final colour. A colour class indexed by $i$ is an [intersecting family](../../../../../intersecting-family.md) because all its members contain $i$; the final class lies in a $(2r-1)$-set and is also intersecting. This proves the upper bound $d+1$.

For the lower bound, first deduce the open-cover [Lusternik-Schnirelmann-Borsuk theorem](../../../../../lusternik-schnirelmann-theorem.md). An [open cover](../../../../../open-cover.md) $U_0,\ldots,U_d$ of $S^d$ admits a continuous [partition of unity](../../../../../partition-of-unity.md) $\phi_0,\ldots,\phi_d$ subordinate to it. Apply the [Borsuk-Ulam theorem](../../../../../borsuk-ulam-theorem.md) to $(\phi_1,\ldots,\phi_d)$. Equal values at $x,-x$ and $\sum_i\phi_i=1$ make all values equal. At least one common value is positive, so some $U_i$ contains an [antipodal pair](../../../../../antipodal-pair.md).

Now suppose the $r$-sets could be coloured with only $d$ colours, each an [intersecting family](../../../../../intersecting-family.md). Choose $N$ points $v_1,\ldots,v_N\in S^d$ such that every $d+1$ of their vectors are [linearly independent](../../../../../linear-independence.md). For example, normalize $(1,t_i,\ldots,t_i^d)$ for distinct real $t_i$; the [Vandermonde determinant](../../../../../vandermonde-determinant.md) proves this property. The [general-position hemisphere count](../../../../../general-position-hemisphere-count.md) says that at most $d$ points lie on any equator. Since $N-d=2r-1$, at least one of the opposite [open hemispheres](../../../../../open-hemisphere.md) determined by $x,-x$ contains an $r$-set of the labelled points.

Let $U_i$ be the open set of directions whose positive [open hemisphere](../../../../../open-hemisphere.md) contains an $r$-set of colour $i$. It contains no [antipodal pair](../../../../../antipodal-pair.md), as such a pair would give two disjoint sets of that colour. The compact set $K=S^d\setminus\bigcup_{i=1}^dU_i$ also contains no [antipodal pair](../../../../../antipodal-pair.md): otherwise each of the two opposite hemispheres would have at most $r-1$ points, contradicting the count $2r-1$.

If $K$ is nonempty, compactness gives a positive [set distance](../../../../../distance-between-two-sets.md) between $K$ and $-K$; an open neighbourhood $U_0$ of radius less than half that [set distance](../../../../../distance-between-two-sets.md) still has no [antipodal pair](../../../../../antipodal-pair.md). If $K$ is empty, take $U_0=\varnothing$. In either case $U_0,U_1,\ldots,U_d$ is an [open cover](../../../../../open-cover.md) with no member containing an [antipodal pair](../../../../../antipodal-pair.md), contradicting the [Lusternik-Schnirelmann-Borsuk theorem](../../../../../lusternik-schnirelmann-theorem.md). Hence at least $d+1$ colours are required.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
