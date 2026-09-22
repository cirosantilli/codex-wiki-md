<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $K=\bigcap_{i\in I}K_i$. Each $K_i$ is [closed](../../../../closed-set.md) in $X$, by the [compact subset of a Hausdorff space](../../../../compact-subset-of-a-hausdorff-space.md) theorem. Therefore $K$ is [closed](../../../../closed-set.md), and is [compact](../../../../compact-space.md) because $X$ is [compact](../../../../compact-space.md). The nonempty finite [intersections](../../../../set-intersection.md) give the [finite intersection property](../../../../finite-intersection-property.md), so part (a)(ii) also yields $K\ne\varnothing$.

Suppose $K$ were not [connected](../../../../connected-space.md). Part (c) would give [disjoint](../../../../disjoint-sets.md) [open sets](../../../../open-set.md) $U,V$ containing $K$ in their [union](../../../../set-union.md) and each meeting $K$. Let

$$
C=X\setminus(U\cup V).
$$

This is a [closed subset](../../../../closed-set.md) of the [compact space](../../../../compact-space.md) $X$, and $C\cap\bigcap_{i\in I}K_i=\varnothing$. Apply the contrapositive of the [finite intersection characterization of compactness](../../../../finite-intersection-characterization-of-compactness.md) to the family of [closed sets](../../../../closed-set.md) $\{C\}\cup\{K_i:i\in I\}$. Some finite subfamily has empty [intersection](../../../../set-intersection.md). Since every finite [intersection](../../../../set-intersection.md) of just the $K_i$ is nonempty, that subfamily must include $C$. Thus for some finite $J\subseteq I$,

$$
C\cap\bigcap_{j\in J}K_j=\varnothing,
\qquad\text{or equivalently}\qquad
K_J:=\bigcap_{j\in J}K_j\subseteq U\cup V.
$$

But $K\subseteq K_J$ and $K$ meets both $U$ and $V$. Therefore $K_J\cap U$ and $K_J\cap V$ are nonempty [disjoint](../../../../disjoint-sets.md) relatively [open sets](../../../../open-set.md) covering $K_J$, contradicting its assumed [connectedness](../../../../connected-space.md). This proves

$$
\boxed{\bigcap_{i\in I}K_i\text{ is nonempty, compact and connected}.}
$$

This is [connectedness of an intersection from connected finite intersections](../../../../connectedness-of-an-intersection-from-connected-finite-intersections.md). If $I=\varnothing$, its [intersection](../../../../set-intersection.md) is $X$; the stated hypothesis for the finite [set](../../../../set-split.md) $J=\varnothing$ already makes $X$ nonempty and [connected](../../../../connected-space.md), so that case is included.

## ↑ Ancestors (12)

1. [D](../d.md)
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
