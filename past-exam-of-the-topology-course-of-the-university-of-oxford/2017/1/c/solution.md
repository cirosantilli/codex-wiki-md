<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [subset](../../../../subset.md) $A$ is [connected](../../../../connected-space.md) when it is a [connected space](../../../../connected-space.md) in its [subspace topology](../../../../subspace-topology.md): there is no [separation of a topological space](../../../../separation-of-a-topological-space.md)

$$
A=P\sqcup Q
$$

into two nonempty [disjoint](../../../../disjoint-sets.md) [open subsets](../../../../open-set.md) of $A$. Equivalently, the only [clopen sets](../../../../clopen-set.md) of $A$ are $\varnothing$ and $A$.

Since the given $A$ is not [connected](../../../../connected-space.md), choose such $P,Q$. Each is the [complement](../../../../complement-of-a-set.md) of the other in $A$, so both are also [closed subsets](../../../../closed-set.md) of $A$. They are [compact](../../../../compact-space.md) by the [closed subset of a compact space](../../../../closed-subset-of-a-compact-space.md) result. We now separate these two [compact subsets](../../../../compact-space.md) by ambient [open sets](../../../../open-set.md).

For each $p\in P$, part (b), applied to $Q$ and $p$, gives [disjoint](../../../../disjoint-sets.md) ambient [open sets](../../../../open-set.md) $G_p,H_p$ with $p\in G_p$ and $Q\subseteq H_p$. Choose $p_1,\ldots,p_m$ such that the $G_{p_j}$ cover $P$, using its [compactness](../../../../compact-space.md). Define

$$
U=\bigcup_{j=1}^mG_{p_j},\qquad
V=\bigcap_{j=1}^mH_{p_j}.
$$

Then $P\subseteq U$, $Q\subseteq V$, and $U,V$ are [disjoint](../../../../disjoint-sets.md) [open sets](../../../../open-set.md). Indeed a point of $U$ lies in some $G_{p_j}$, whereas every point of $V$ lies in the corresponding $H_{p_j}$. Consequently

$$
\boxed{A\subseteq U\cup V,\qquad A\cap U=P\ne\varnothing,\qquad A\cap V=Q\ne\varnothing.}
$$

This proves the requested ambient separation, using the more general [separation of disjoint compact subsets](../../../../separation-of-disjoint-compact-subsets.md). The initially given relatively [open sets](../../../../open-set.md) $P,Q$ need not themselves be [open](../../../../open-set.md) in $X$; the finite construction supplies ambient [open neighbourhoods](../../../../open-neighbourhood.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
