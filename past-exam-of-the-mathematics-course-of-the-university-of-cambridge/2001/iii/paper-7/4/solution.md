<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [group](../../../../../group-split.md) $G(K)$ consists of the nonvanishing [continuous functions](../../../../../continuous-function.md), and $E(K)$ is a [subgroup](../../../../../subgroup.md) because multiplication is commutative: $e^ge^h=e^{g+h}$. The objective is a logarithm decomposition with finitely many integer obstructions, one for each bounded complementary component. No local connectivity of $K$ is assumed.

We use two elementary finite-neighborhood facts, which make the outline independent of the general Jordan theorem. Given a neighborhood $V$ of $K$, take a finite grid neighborhood $N\subset V$ with $K\subset\operatorname{int}N$. It can be chosen to be a finite union of polygonal surfaces with [boundary](../../../../../boundary-of-a-set.md). Its complement has finitely many bounded holes. Holes that lie in the same component of $\mathbb C\setminus K$ can be joined by thin polygonal corridors disjoint from $K$, which are removed from $N$. A hole lying in the unbounded component is similarly joined to the exterior. For the remaining finitely many components, corridors may be continued to include their chosen representatives $a_i$. Small polygonal adjustments preserve $K\subset\operatorname{int}N$ and $N\subset V$. Thus every remaining bounded hole lies in a distinct bounded component of $\mathbb C\setminus K$ and contains its representative. One may also arrange this for any prescribed finite list of bounded components by first keeping their representative points out of the grid neighborhood. All paths used are [compact](../../../../../compact-space.md) and disjoint from $K$, so sufficiently thin corridors remain disjoint from $K$.

For such a finite polygonal $N$, winding indices identify the [homology group](../../../../../homology-group.md) $H_1(N;\mathbb Z)$ with the [free abelian group](../../../../../free-abelian-group.md) on its bounded holes. Here is a finite-chain explanation. Triangulate a large disc with $N$ as a subcomplex. Every integral one-cycle bounds a two-chain in the disc. Its filling coefficient is constant on each component of the complement of $N$, is zero on the exterior, and is the winding index there. If all bounded-hole indices vanish, the filling is supported in $N$, so the cycle already bounds in $N$. Conversely the sum of the oriented faces in one hole has its chain boundary in $N$ and has index one in that hole and zero in the others. Thus cycles $\gamma_j$ can be chosen with $\operatorname{wind}(\gamma_j,a_i)=\delta_{ij}$. These can be integral sums of [boundary](../../../../../boundary-of-a-set.md) curves, which matters when components of $N$ are nested. This proves the needed statement using finite triangulation, not separation of an arbitrary simple [closed](../../../../../closed-set.md) curve. Together these are [finite-hole neighborhoods of a planar compact set](../../../../../finite-hole-neighborhoods-of-a-planar-compact-set.md).

Now extend $f\in G(K)$ to a continuous $F$ near $K$, using the [Tietze extension theorem](../../../../../tietze-extension-theorem.md) on its real and imaginary parts. Since $\min_K|f|>0$, shrink the neighborhood until $F$ has no zeros, and choose $N$ within it as above. The winding of $F$ on the cycles $\gamma_j$ defines integers $k_j$. Set

$$
r(z)=\prod_j(z-a_j)^{k_j},
$$

where only the finitely many represented holes are used. The winding of $F/r$ on every cycle of $N$ is zero. On each component choose a local [complex logarithm](../../../../../complex-logarithm.md) at a base point and continue it along paths. Zero [winding number](../../../../../winding-number.md) around every loop makes the continued value independent of the path; local logarithm charts make it continuous. The [continuous logarithm lifting criterion](../../../../../continuous-logarithm-lifting-criterion.md) therefore gives $F/r=e^g$ on $N$, and restriction gives $f=e^{g|_K}r|_K$. Thus $G(K)=E(K)G(\mathbf a)$, even when $K$ has infinitely many holes: each individual function uses finitely many factors.

To prove uniqueness, suppose a finite product $r=\prod(z-a_i)^{k_i}$ equals $e^g$ on $K$. Extend $g$ continuously to a neighborhood. There $re^{-g}$ is close to $1$ after shrinking, so it has its small-branch logarithm. Hence $r$ itself has a [continuous function](../../../../../continuous-function.md) giving a [complex logarithm](../../../../../complex-logarithm.md) on that neighborhood. Choose $N$ there detecting all the finitely many $a_i$ as separate holes. Its dual cycles give $\operatorname{wind}(r\circ\gamma_j,0)=k_j$, while a function with a logarithm has zero [winding number](../../../../../winding-number.md). Therefore every $k_j=0$. This proves both freeness of the listed [rational functions](../../../../../rational-function.md) and $E(K)\cap G(\mathbf a)=\{1\}$. All subgroups commute, so

$$
\boxed{G(K)=E(K)\times G(\mathbf a),\qquad G(K)/E(K)\cong\bigoplus_{\text{bounded }U\subset\mathbb C\setminus K}\mathbb Z}.
$$

This is [planar logarithm factorization](../../../../../planar-logarithm-factorization.md). If there are no bounded components the second factor is trivial.

For the Jordan curve deduction, let $J$ be homeomorphic to the circle. Parametrize it by $\gamma:[0,1]\to J$ with just the two endpoints identified. For $f\in G(J)$, lift a logarithm of $f\circ\gamma$ along the interval. Its endpoint increment is $2\pi i n$. The integer $n$ is additive, every integer is attained by a function with $f(\gamma(t))=e^{2\pi int}$, and $n=0$ precisely when the lift descends to a logarithm on $J$. Hence $G(J)/E(J)\cong\mathbb Z$. The factorization says this is free abelian on the bounded complementary components; comparison of ranks, or tensoring with $\mathbb Q$, shows that exactly one bounded component exists. There is also the unique unbounded component, so the complement has exactly two components.

We still need the common-boundary assertion. A proper [closed](../../../../../closed-set.md) arc has trivial exponential quotient because every nonvanishing function on an interval admits a logarithm. Factorization consequently makes the complement of such an arc connected, and since it is [open](../../../../../open-set.md) it is [path-connected](../../../../../path-connected-space.md). Fix $p\in J$ and any neighborhood $V$ of $p$, and choose a small [open](../../../../../open-set.md) arc $A\subset J\cap V$ containing $p$. The remainder $J\setminus A$ is a proper [closed](../../../../../closed-set.md) arc. Join a point in each of the two complementary components by a path avoiding $J\setminus A$. This path must meet $J$, and every such meeting lies in $A$. The segment before its first meeting lies in the first region, and the segment after its last meeting lies in the second; [continuity](../../../../../continuous-function.md) makes both regions meet $V$. Thus every point of $J$ lies on both boundaries. Conversely either [boundary](../../../../../boundary-of-a-set.md) is contained in the [closed](../../../../../closed-set.md) set $J$. **There are exactly two regions, one bounded and one unbounded, with common [boundary](../../../../../boundary-of-a-set.md) $J$**, the [Jordan curve theorem](../../../../../jordan-curve-theorem.md). This is [Jordan separation from the exponential quotient](../../../../../jordan-separation-from-the-exponential-quotient.md); it does not assume the theorem in the factorization proof.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
