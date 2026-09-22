# Connected complement of a product of proper subsets

↑ **Parent:** [Connected space](connected-space.md)

Suppose $X,Y$ are nonempty [connected spaces](connected-space.md), and $A\subsetneq X$, $B\subsetneq Y$ are proper [subsets](subset.md). Then $C=(X\times Y)\setminus(A\times B)$, with its [subspace topology](subspace-topology.md) from the [product topology](product-topology.md), is a [connected space](connected-space.md). No [closed set](closed-set.md) or [open set](open-set.md) hypothesis on $A,B$ is needed.

Choose $x_0\in X\setminus A$, $y_0\in Y\setminus B$. The two [topological subspaces](topological-subspace.md) $\{x_0\}\times Y$ and $X\times\{y_0\}$ are [homeomorphic](homeomorphism.md) to the factors, intersect at $(x_0,y_0)$, and lie in $C$. Their [union](set-union.md) is a [connected subset](connected-subset.md) $H$. Every $(x,y)\in C$ has $x\notin A$ or $y\notin B$. In the first case its entire vertical copy $\{x\}\times Y$ lies in $C$ and meets $H$; in the second case the horizontal copy $X\times\{y\}$ does so. Thus $C$ is a [connected union with a connected hub](connected-union-with-a-connected-hub.md).

Both properness assumptions are needed for this general result. Taking $X=Y=\mathbb R$, $A=X$ and $B=\{0\}$ gives the two disjoint [open](open-set.md) half-planes $y<0$ and $y>0$, a [separation of a topological space](separation-of-a-topological-space.md) of the complement.

## ↑ Ancestors (5)

1. [Connected space](connected-space.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
