<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the external [external vertex boundary](../../../../../external-vertex-boundary.md) convention

$$
B(\mathcal A)=\{X\notin\mathcal A:\ |X\mathbin\triangle A|=1\text{ for some }A\in\mathcal A\}.
$$

Equivalently, its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) is $N[\mathcal A]=\mathcal A\cup B(\mathcal A)$. Some boundary conventions use this [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) itself; because the compared [set families](../../../../../set-family.md) have equal size, either convention gives the same inequality.

Order the [Boolean lattice](../../../../../boolean-lattice.md) first by increasing size, and within a size by [lexicographic order](../../../../../lexicographic-order.md), with the smallest differing coordinate in the earlier set. If $I$ is the [initial segment](../../../../../initial-segment.md) in this [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md) with $|I|=|\mathcal A|$, [Harper inequality](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) is

$$
\boxed{|B(\mathcal A)|\geq|B(I)|},
\qquad\text{equivalently}\qquad |N[\mathcal A]|\geq|N[I]|.
$$

In particular, writing $S_n(t)=\sum_{j=0}^t\binom nj$, if $|\mathcal A|\geq S_n(t)$ then $|N[\mathcal A]|\geq S_n(t+1)$.

Here is the full [simplicial section compression](../../../../../simplicial-section-compression.md) proof. The cases $n=0,1$ are immediate. A simplicial [initial segment](../../../../../initial-segment.md) has an initial-segment [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md): it contains every smaller level, and its remaining upper level is the [upper shadow](../../../../../upper-shadow.md) of a [lexicographic](../../../../../lexicographic-order.md) [initial segment](../../../../../initial-segment.md). That [upper shadow](../../../../../upper-shadow.md) is [lexicographic](../../../../../lexicographic-order.md) initial because a set has a face in the segment exactly when its earliest face does, and earliest faces preserve [lexicographic order](../../../../../lexicographic-order.md).

Assume the result in dimension $n-1$. For a coordinate $i$, delete it from the present section and write the two sections as $\mathcal A_0,\mathcal A_1$. Their neighbourhood sections are exactly

$$
N[\mathcal A]_0=N[\mathcal A_0]\cup\mathcal A_1,
\qquad N[\mathcal A]_1=N[\mathcal A_1]\cup\mathcal A_0.
$$

Replace both sections by equally large simplicial [initial segments](../../../../../initial-segment.md) $I_0,I_1$. The [mathematical induction](../../../../../mathematical-induction.md) hypothesis controls each internal neighbourhood. Both sets in each new union are [initial segments](../../../../../initial-segment.md), so that union has size equal to the larger of their sizes. The corresponding old union has at least that size. Therefore this [simplicial section compression](../../../../../simplicial-section-compression.md) does not enlarge $N[\mathcal A]$.

Repeatedly compress any noninitial section. Every change strictly reduces the sum of the global simplicial positions of the [set family](../../../../../set-family.md) members, so the process terminates at a [set family](../../../../../set-family.md) $\mathcal C$ compressed in every section. Suppose an earlier [vertex](../../../../../vertex-graph-theory.md) $X$ is missing while a later [vertex](../../../../../vertex-graph-theory.md) $Y$ is present. If they agree in any coordinate, they contradict compression of that coordinate's section. Thus $Y=[n]\setminus X$. They must also be consecutive in simplicial order: an intermediate [vertex](../../../../../vertex-graph-theory.md), whether present or absent, would create another inversion and would have to equal one of these two complementary [vertices](../../../../../vertex-graph-theory.md). No other inversion is possible for the same reason. Hence $\mathcal C$ is either the required [initial segment](../../../../../initial-segment.md) or that segment with its last [vertex](../../../../../vertex-graph-theory.md) $X$ exchanged for the next [vertex](../../../../../vertex-graph-theory.md) $Y$, with $X,Y$ complementary.

For completeness, these [terminal families for simplicial section compression](../../../../../terminal-families-for-simplicial-section-compression.md) can be checked explicitly. If $n=2k+1$, the exceptional consecutive [vertices](../../../../../vertex-graph-theory.md) are the last $k$-set $X=\{k+2,\ldots,2k+1\}$ and first $(k+1)$-set $Y=\{1,\ldots,k+1\}$. For $k\geq1$, the [initial segment](../../../../../initial-segment.md) is all levels through $k$. After the exchange every [vertex](../../../../../vertex-graph-theory.md) of size at most $k+1$ is still in its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md): a $(k+1)$-set has at least two $k$-faces, so deleting the one face $X$ cannot remove it, and $X$ itself neighbours a retained smaller set. Thus the new neighbourhood contains the old one. For $k=0$, the two single-vertex [set families](../../../../../set-family.md) have the same neighbourhood.

If $n=2k$, the exceptional pair is $X=\{1,k+2,\ldots,2k\}$ and $Y=\{2,\ldots,k+1\}$. The [initial segment](../../../../../initial-segment.md) consists of every level below $k$ and all $k$-sets containing coordinate one. Its [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) consists of every level through $k$ and the $(k+1)$-sets containing coordinate one. For $k\geq2$, each of the latter has $k\geq2$ faces containing coordinate one, so deleting $X$ removes no such neighbour. Every lower level remains covered. For $k=1$, the added [vertex](../../../../../vertex-graph-theory.md) $Y$ itself keeps the sole two-element neighbour covered. Again the exchange does not decrease the neighbourhood. These are the only complementary consecutive pairs, as is seen by checking the central ranks and the [lexicographic](../../../../../lexicographic-order.md) transition between middle-rank sets containing and avoiding coordinate one.

We have reached a [set family](../../../../../set-family.md) whose neighbourhood is at least the [initial segment](../../../../../initial-segment.md)'s, without increasing the original neighbourhood. This proves [Harper inequality](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) by [mathematical induction](../../../../../mathematical-induction.md), including the exceptional compressed [set families](../../../../../set-family.md) often omitted from the argument.

For the final request, **the usual two-coordinate shift does not increase the boundary of a [uniform set family](../../../../../uniform-set-family.md).** To see this carefully, let $i\neq j$ and let $C_{ij}$ move a set containing $j$ but not $i$ to its partner with $j$ replaced by $i$, only if that partner is absent. For any [uniform set family](../../../../../uniform-set-family.md) $\mathcal F$,

$$
\partial(C_{ij}\mathcal F)\subseteq C_{ij}(\partial\mathcal F),
\qquad
\nabla(C_{ij}\mathcal F)\subseteq C_{ij}(\nabla\mathcal F).
$$

Here is the local witness check for the [lower shadow](../../../../../lower-shadow.md) inclusion. A shadow member containing neither or both of $i,j$ has an old witness after possibly exchanging $i,j$ in that witness. For a paired shadow [vertex](../../../../../vertex-graph-theory.md) containing $i$ only, either its old version or its $j$-partner has an old witness, which suffices for its membership in the shifted shadow. For a [vertex](../../../../../vertex-graph-theory.md) containing $j$ only that survives in the new shadow, its new witness either contains both coordinates, supplying both old shadow partners directly, or is an unshifted $j$-only witness whose $i$-partner was already present. In either event both old shadow partners existed, which is exactly the condition for the $j$-vertex to survive the shadow shift. This exhausts the coordinate patterns.

Taking complements converts an [upper shadow](../../../../../upper-shadow.md) into a [lower shadow](../../../../../lower-shadow.md) and converts $C_{ij}$ into $C_{ji}$, proving the second inclusion. Each shift preserves [cardinality](../../../../../cardinality.md) on the shadow level. The external boundary of an $r$-uniform [set family](../../../../../set-family.md) is the disjoint union of its lower and upper shadows, so

$$
\boxed{|B(C_{ij}\mathcal F)|=|\partial C_{ij}\mathcal F|+|\nabla C_{ij}\mathcal F|
\leq|\partial\mathcal F|+|\nabla\mathcal F|=|B(\mathcal F)|.}
$$

The endpoint levels $r=0,n$ have an empty shadow on one side and obey the same conclusion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
