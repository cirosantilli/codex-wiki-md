# Every subset of a cofinite space is compact

↑ **Parent:** [Cofinite topology](cofinite-topology.md)

Every [subset](subset.md) $A$ of a [cofinite](cofinite-set.md) [topological space](topological-space.md) is a [compact subset](compact-space.md). To see the finite reduction directly, take an [open cover](open-cover.md) of a nonempty $A$ by [open sets](open-set.md) of $X$ and choose one member $U$ containing a point of $A$. Since $U$ has finite [complement](complement-of-a-set.md), the [set](set-split.md) $A\setminus U$ is finite. Choose a covering member for each of those remaining points. Those members together with $U$ are a [finite subcover](finite-subcover.md). The [empty set](empty-set.md) is already [compact](compact-space.md).

Equivalently, the [subspace topology](subspace-topology.md) on $A$ is itself cofinite: for finite $F\subseteq X$, the trace of $X\setminus F$ is $A\setminus(F\cap A)$. The argument applies again inside $A$. A concrete [open cover](open-cover.md) $\{X\setminus\{k\}:k\in X\}$ of $X=\mathbb N_{>0}$ needs only the two members $X\setminus\{1\}$ and $X\setminus\{2\}$ when these labels are distinct: each fills the other's single gap.

On $X=\mathbb N_{>0}$, the [subset](subset.md) of [even integers](even-number.md) is [compact](compact-space.md) but not [closed](closed-set.md), because it is infinite and proper. A [compact subset of a Hausdorff space](compact-subset-of-a-hausdorff-space.md) is guaranteed to be [closed](closed-set.md), whereas [compactness](compact-space.md) without the [Hausdorff space](hausdorff-space.md) assumption does not suffice. Changing the [topology](topology-split.md) changes [compactness](compact-space.md): the same infinite [set](set-split.md) with its [discrete topology](discrete-space.md) has the [singleton](singleton-mathematics.md) [open cover](open-cover.md), which has no [finite subcover](finite-subcover.md). The finite-exception argument is special to finite [complements](complement-of-a-set.md); in the [cocountable topology](countable-complement-topology.md), [compact subsets of a cocountable space](compact-subsets-of-a-cocountable-space.md) must instead be finite.

## ↑ Ancestors (6)

1. [Cofinite topology](cofinite-topology.md)
2. [Topology](topology-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cofinite topology](cofinite-topology.md)
