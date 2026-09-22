<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We derive the [triangle removal lemma](../../../../../triangle-removal-lemma.md) from the permitted [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md), then turn a [corner in an integer grid](../../../../../corner-in-an-integer-grid.md) into a [triangle in a graph](../../../../../triangle-in-a-graph.md).

The [triangle removal lemma](../../../../../triangle-removal-lemma.md) says that for every $\eta>0$ there are $\rho>0$ and $N_0$ such that a [graph](../../../../../graph-split.md) on $N\geq N_0$ [vertices](../../../../../vertex-graph-theory.md) with fewer than $\rho N^3$ [triangles in a graph](../../../../../triangle-in-a-graph.md) can be made [triangle-free](../../../../../triangle-free-graph.md) by deleting at most $\eta N^2$ [edges](../../../../../edge-of-a-graph.md). Here [triangles in a graph](../../../../../triangle-in-a-graph.md) are unordered triples of distinct [vertices](../../../../../vertex-graph-theory.md). We prove this consequence with the necessary quantitative dependence.

We may assume $0<\eta<1$. Put $d=\eta/4$, choose an integer $m_0\geq4/\eta$, and choose

$$
0<\varepsilon\leq\min\{\eta/8,d/4,1/4\}.
$$

Apply the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) to obtain an exceptional class $V_0$ of size at most $\varepsilon N$ and equal-sized classes $V_1,\ldots,V_k$ of size $L$, where $m_0\leq k\leq M$, and at most $\varepsilon k^2$ pairs are not [regular pairs of vertex sets](../../../../../regular-pair-of-vertex-sets.md). The constant $M$ depends only on these chosen parameters. Delete all [edges](../../../../../edge-of-a-graph.md) incident with $V_0$, all [edges](../../../../../edge-of-a-graph.md) within a class, all [edges](../../../../../edge-of-a-graph.md) between irregular pairs, and all [edges](../../../../../edge-of-a-graph.md) between pairs whose [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) is less than $d$. The respective costs are at most

$$
\varepsilon N^2,\qquad \frac{N^2}{2m_0},\qquad \varepsilon N^2,\qquad \frac d2N^2.
$$

Their sum is at most $\eta N^2/2$, hence certainly at most $\eta N^2$.

If a [triangle in a graph](../../../../../triangle-in-a-graph.md) survives, it lies in three distinct classes whose three pairs are $\varepsilon$-[regular pairs of vertex sets](../../../../../regular-pair-of-vertex-sets.md) of [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) at least $d$ in the original [graph](../../../../../graph-split.md). We now check the needed [regular triangle counting lemma](../../../../../regular-triangle-counting-lemma.md). In the first class all but at most $2\varepsilon L$ [vertices](../../../../../vertex-graph-theory.md) have at least $(d-\varepsilon)L$ neighbours in each of the other two classes; otherwise the definition of a [regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md) would be violated. For each such [vertex](../../../../../vertex-graph-theory.md) $v$, its two neighbour sets each have size at least $\varepsilon L$, so their mutual [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) is at least $d-\varepsilon$. It follows that the original three classes contain at least

$$
(1-2\varepsilon)(d-\varepsilon)^3L^3\geq\frac{d^3}{8}L^3
$$

[triangles in a graph](../../../../../triangle-in-a-graph.md). The elementary lower bound holds because $\varepsilon\leq1/4$ and $\varepsilon\leq d/4$. Also $L=(N-|V_0|)/k\geq N/(2M)$. Thus a surviving [triangle in a graph](../../../../../triangle-in-a-graph.md) implies at least $d^3N^3/(64M^3)$ original [triangles in a graph](../../../../../triangle-in-a-graph.md). Set $\rho=d^3/(128M^3)$ and take $N_0$ large enough for the [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md). Fewer than $\rho N^3$ original [triangles in a graph](../../../../../triangle-in-a-graph.md) force the cleaned [graph](../../../../../graph-split.md) to be [triangle-free](../../../../../triangle-free-graph.md), proving the [triangle removal lemma](../../../../../triangle-removal-lemma.md).

Now suppose $0<\delta\leq1$ and $A\subseteq[n]^2$. Use the [tripartite graph encoding of a grid](../../../../../tripartite-graph-encoding-of-a-grid.md) to construct a [tripartite graph](../../../../../tripartite-graph.md) with disjoint labelled classes

$$
X=[n],\qquad Y=[n],\qquad Z=[2n].
$$

For each $(a,b)\in A$, put in the three [edges](../../../../../edge-of-a-graph.md) joining $a\in X$, $b\in Y$, and $a+b\in Z$. These yield $|A|$ canonical [triangles in a graph](../../../../../triangle-in-a-graph.md). They are pairwise [edge-disjoint triangles](../../../../../edge-disjoint-triangles.md): an $XY$ [edge](../../../../../edge-of-a-graph.md) determines $(a,b)$ directly, an $XZ$ [edge](../../../../../edge-of-a-graph.md) determines $b=z-a$, and a $YZ$ [edge](../../../../../edge-of-a-graph.md) determines $a=z-b$. Any deletion making the [graph](../../../../../graph-split.md) [triangle-free](../../../../../triangle-free-graph.md) must therefore remove at least $|A|$ [edges](../../../../../edge-of-a-graph.md).

On the other hand, an arbitrary [triangle in a graph](../../../../../triangle-in-a-graph.md) with labels $(x,y,z)$ gives three points of $A$:

$$
(x,y),\qquad(x,z-x),\qquad(z-y,y).
$$

Writing $d=z-x-y$, these are $(x,y),(x,y+d),(x+d,y)$. If $d\ne0$, they form the required [corner in an integer grid](../../../../../corner-in-an-integer-grid.md). If there is no such [corner in an integer grid](../../../../../corner-in-an-integer-grid.md), every [triangle in a graph](../../../../../triangle-in-a-graph.md) is canonical, and the total number is precisely $|A|\leq n^2$.

Apply the [triangle removal lemma](../../../../../triangle-removal-lemma.md) with $\eta=\delta/32$. The constructed [graph](../../../../../graph-split.md) has $N=4n$ [vertices](../../../../../vertex-graph-theory.md). For sufficiently large $n$, $N\geq N_0$ and

$$
n^2<\rho(4n)^3.
$$

In the absence of a [corner in an integer grid](../../../../../corner-in-an-integer-grid.md), the [triangle removal lemma](../../../../../triangle-removal-lemma.md) would destroy all [triangles in a graph](../../../../../triangle-in-a-graph.md) by deleting at most

$$
\eta(4n)^2=\frac\delta2n^2<\delta n^2\leq|A|
$$

[edges](../../../../../edge-of-a-graph.md), contradicting the pairwise [edge-disjoint triangles](../../../../../edge-disjoint-triangles.md). **Every sufficiently large grid therefore has the asserted [corner in an integer grid](../../../../../corner-in-an-integer-grid.md) in every subset of positive fixed [density of a finite subset](../../../../../density-of-a-finite-subset.md).** For $\delta>1$ there is no eligible subset, so the assertion is vacuous. This proves the [corners theorem](../../../../../corners-theorem.md), including the stipulated nonzero displacement; no positivity of $d$ was required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
