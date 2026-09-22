<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $x$ in a [compact Hausdorff space](../../../../compact-hausdorff-space.md) $K$, its [quasi-component](../../../../quasi-component.md) $Q$ is the intersection of all [clopen sets](../../../../clopen-set.md) containing $x$. It is closed and therefore [compact](../../../../compact-space.md). Suppose $Q=A\sqcup B$ is a [separation of a topological space](../../../../separation-of-a-topological-space.md) into two nonempty relatively [closed sets](../../../../closed-set.md), with $x\in A$. The sets $A,B$ are [compact](../../../../compact-space.md) and hence closed in $K$. [Normality of a compact Hausdorff space](../../../../normality-of-a-compact-hausdorff-space.md) gives disjoint [open neighborhoods](../../../../open-neighbourhood.md) $U,V$ of $A,B$.

The [compact set](../../../../compact-space.md) $K\setminus(U\cup V)$ is disjoint from $Q$. For each [point](../../../../point-geometry.md) $y$ of that set choose a [clopen](../../../../clopen-set.md) $C_y$ containing $x$ but not $y$. Finitely many complements cover $K\setminus(U\cup V)$, so their corresponding intersection $C$ is [clopen](../../../../clopen-set.md), contains $Q$, and is contained in $U\cup V$. Now $C\cap U$ is [clopen](../../../../clopen-set.md) in $C$, hence [clopen](../../../../clopen-set.md) in $K$, and contains $x$ while missing $B$. This contradicts the definition of $Q$. Thus **$Q$ is [connected](../../../../connected-space.md)**. Any [connected set](../../../../connected-set.md) containing $x$ lies in every [clopen](../../../../clopen-set.md) [neighborhood](../../../../neighbourhood-mathematics.md) of $x$, so the [connected component](../../../../connected-component.md) of $x$ equals $Q$.

For the second assertion, $D$ is closed in the ambient [Hausdorff space](../../../../hausdorff-space.md) $X$, and is itself [compact](../../../../compact-space.md) [Hausdorff](../../../../hausdorff-space.md). Let $C$ be a [connected component](../../../../connected-component.md) of $D$ disjoint from $\partial_XD$. Choose $p\in C$. By the first assertion $C$ is the [quasi-component](../../../../quasi-component.md) of $p$ in $D$. For each $y\in\partial_XD$ choose a [clopen](../../../../clopen-set.md) subset of $D$ containing $p$ but not $y$. [Compactness](../../../../compact-space.md) of $\partial_XD\subseteq D$ gives a [finite intersection](../../../../finite-intersection.md) $H$ of these sets which contains $C$ and avoids the whole [boundary](../../../../boundary-of-a-set.md). Thus $H\subseteq\operatorname{int}_XD$. It is closed in $X$, because it is closed in the [closed set](../../../../closed-set.md) $D$, and is open in $X$, because it is relatively open in $D$ and contained in its [interior](../../../../interior-topology.md). It is nonempty and proper, contradicting [connectedness](../../../../connected-space.md) of $X$. Hence **every [connected component](../../../../connected-component.md) of $D$ meets its [boundary](../../../../boundary-of-a-set.md)**.

Finally suppose a closed subset $A$ of the square has the [point](../../../../point-geometry.md)-separating [clopen](../../../../clopen-set.md) property specified in the paper. Every nonempty relatively open subset of the square contains a nontrivial [line segment](../../../../line-segment.md): it contains an [interior](../../../../interior-topology.md) [point](../../../../point-geometry.md) of the square and a small ball about that [point](../../../../point-geometry.md). If such a segment lay in $A$, a [clopen](../../../../clopen-set.md) subset of $A$ separating its endpoints would induce a [separation of a topological space](../../../../separation-of-a-topological-space.md) of the [connected](../../../../connected-space.md) segment. This is impossible. Therefore $A$ contains no nonempty relatively open subset of the square. Being closed, it is **[nowhere dense](../../../../nowhere-dense-set.md) in the square**, and also [nowhere dense](../../../../nowhere-dense-set.md) in $\mathbb R^2$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
