<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every $k\in K$, the [Hausdorff condition](../../../../hausdorff-space.md) gives [disjoint](../../../../disjoint-sets.md) [open neighbourhoods](../../../../open-neighbourhood.md) $U_k$ of $k$ and $V_k$ of $x$. The $U_k$ form an [open cover](../../../../open-cover.md) of $K$, so choose a [finite subcover](../../../../finite-subcover.md) $U_{k_1},\ldots,U_{k_m}$. Put

$$
U=\bigcup_{j=1}^mU_{k_j},\qquad V=\bigcap_{j=1}^mV_{k_j}.
$$

Then $U,V$ are [open sets](../../../../open-set.md), $K\subseteq U$ and $x\in V$. If a point belonged to $U\cap V$, it would belong to some $U_{k_j}$ and to $V_{k_j}$, contrary to their choice. Thus

$$
\boxed{K\subseteq U,\qquad x\in V,\qquad U\cap V=\varnothing.}
$$

The finiteness matters: a finite [intersection](../../../../set-intersection.md) of [open sets](../../../../open-set.md) is [open](../../../../open-set.md). This is [separation of a point and a compact set](../../../../separation-of-a-point-and-a-compact-set.md). If $K=\varnothing$, use $U=\varnothing$, $V=X$.

Every $x\in X\setminus K$ consequently has an [open neighbourhood](../../../../open-neighbourhood.md) $V$ contained in $X\setminus K$. The [complement](../../../../complement-of-a-set.md) is [open](../../../../open-set.md), so **a [compact subset of a Hausdorff space](../../../../compact-subset-of-a-hausdorff-space.md) is [closed](../../../../closed-set.md)**.

**The conclusion can fail without the [Hausdorff condition](../../../../hausdorff-space.md).** Take the two-point [set](../../../../set-split.md) $X=\{0,1\}$ with the [indiscrete topology](../../../../indiscrete-topology.md) $\{\varnothing,X\}$. The [singleton](../../../../singleton-mathematics.md) $K=\{0\}$ is [compact](../../../../compact-space.md), since one member of any [open cover](../../../../open-cover.md) suffices. It is not [closed](../../../../closed-set.md), because its [complement](../../../../complement-of-a-set.md) $\{1\}$ is not [open](../../../../open-set.md). The two points cannot have [disjoint](../../../../disjoint-sets.md) [open neighbourhoods](../../../../open-neighbourhood.md), so this example is indeed not [Hausdorff](../../../../hausdorff-space.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the topology course of the University of Oxford](../../../split.md)
5. [Topology course of the University of Oxford](../../../../topology-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
