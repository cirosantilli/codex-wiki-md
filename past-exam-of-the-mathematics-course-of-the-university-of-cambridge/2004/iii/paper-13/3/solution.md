<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $t$ be the maximum number of positive [Euclidean distances](../../../../../euclidean-distance.md) from one of the $n$ points to the others. It suffices to prove the stronger [Székely distinct-distance bound](../../../../../szekely-distinct-distance-bound.md), $t\geq cn^{4/5}$. Here $n\geq2$; enlarge constants to handle bounded $n$.

First prove the [crossing lemma for multigraphs](../../../../../crossing-lemma-for-multigraphs.md). In an optimal drawing of a loopless [multigraph](../../../../../multigraph.md) with $v$ [vertices](../../../../../vertex-graph-theory.md), $e$ [edges](../../../../../edge-of-a-graph.md) and maximum parallel multiplicity $\mu$, crossings of incident [edges](../../../../../edge-of-a-graph.md) can be removed by interchanging initial segments, so each remaining crossing involves four distinct [vertices](../../../../../vertex-graph-theory.md). In each parallel class choose one of its [edges](../../../../../edge-of-a-graph.md) with probability $1/\mu$ per [edge](../../../../../edge-of-a-graph.md), selecting none with the remaining probability. Independently keep each [vertex](../../../../../vertex-graph-theory.md) with probability $p$. The resulting [simple graph](../../../../../simple-graph.md) has expected [edge](../../../../../edge-of-a-graph.md) count $p^2e/\mu$, expected [vertex](../../../../../vertex-graph-theory.md) count $pv$, and expected crossings $p^4X/\mu^2$, where $X$ is the original crossing count. Deleting one [edge](../../../../../edge-of-a-graph.md) per crossing and using the allowed [planar graph edge bound](../../../../../planar-graph-edge-bound.md) yields

$$
\frac{p^4X}{\mu^2}\geq\frac{p^2e}{\mu}-3pv.
$$

If $e\geq4\mu v$, take $p=4\mu v/e$ to obtain

$$
X\geq\frac{e^3}{64\mu v^2}.
$$

The case $\mu=1$ is the ordinary [crossing lemma](../../../../../crossing-lemma.md).

We also need the [rich line bound](../../../../../rich-line-bound.md). Given $L$ [lines](../../../../../straight-line.md), connect consecutive incidence points on each [line](../../../../../straight-line.md) by straight [edges](../../../../../edge-of-a-graph.md). This [simple graph](../../../../../simple-graph.md) has at least $I-L$ [edges](../../../../../edge-of-a-graph.md), where $I$ is the total number of incidences, and at most $L^2$ crossings. The [crossing lemma](../../../../../crossing-lemma.md) gives $I=O((nL)^{2/3}+n+L)$, proving the [Szemerédi–Trotter theorem](../../../../../szemeredi-trotter-theorem.md) here rather than assuming it. For [lines](../../../../../straight-line.md) containing at least $k$ points, $I\geq kL$, and absorbing the additive $L$ term gives

$$
L_{\geq k}=O(n^2/k^3+n/k),\qquad k\geq2.
$$

For bounded $k$, counting point pairs gives the same estimate with a larger absolute constant. Grouping rich [lines](../../../../../straight-line.md) into occupancy ranges $2^jk\leq s<2^{j+1}k$ and summing the resulting geometric series proves

$$
\sum_{\ell:\,|P\cap\ell|\geq k}|P\cap\ell|
=O(n^2/k^2+n\log n).
$$

Now form the [circular-arc graph for distinct distances](../../../../../circular-arc-graph-for-distinct-distances.md). Around every point draw each positive-distance [circle](../../../../../circle.md) centred there; there are at most $nt$ such [circles](../../../../../circle.md). A [circle](../../../../../circle.md) with at least three of the original points contributes one [edge](../../../../../edge-of-a-graph.md) between each consecutive pair around it. Discard the [circles](../../../../../circle.md) with at most two points. Since the total number of centre-to-point incidences is $n(n-1)$, the remaining loopless [multigraph](../../../../../multigraph.md) has

$$
e\geq n(n-1)-2nt.
$$

Its circular-arc drawing has $O(n^2t^2)$ crossings: two distinct [circles](../../../../../circle.md) have at most two intersections, and small perturbations remove tangencies and multiple crossings without changing this order.

The apparent difficulty is unbounded parallel multiplicity. The [rich-bisector deletion bound](../../../../../rich-bisector-deletion-bound.md) controls it. Every centre supporting an arc between fixed endpoints lies on their [perpendicular bisector](../../../../../perpendicular-bisector.md). Distinct parallel arcs come from distinct centres, since their common endpoints determine the radius once the centre is fixed. Thus multiplicity at least $k$ makes that [line](../../../../../straight-line.md) contain at least $k$ of the points. For a [line](../../../../../straight-line.md) with $s$ centres, each of its at most $st$ [circles](../../../../../circle.md) has at most two consecutive-point arcs symmetric about that [line](../../../../../straight-line.md), one at each end of its diameter along the [line](../../../../../straight-line.md). The occupancy sum above therefore bounds the number of high-multiplicity arcs by

$$
O(tn^2/k^2+tn\log n).
$$

If $t\geq n^{4/5}$ there is nothing to prove. Otherwise $t\log n=o(n)$ and $t=o(n)$. Choose $k=\lceil K\sqrt t\rceil$ with a sufficiently large absolute constant $K$. The first deletion term is at most a small fixed fraction of $n^2$ and the second is $o(n^2)$. A remaining [multigraph](../../../../../multigraph.md) therefore has $e_1\geq c_1n^2$ [edges](../../../../../edge-of-a-graph.md) and multiplicity at most $k$. For large $n$, $e_1\geq4kn$, so the [crossing lemma for multigraphs](../../../../../crossing-lemma-for-multigraphs.md) gives

$$
Cn^2t^2\geq X_1\geq\frac{e_1^3}{64kn^2}
\geq c_2\frac{n^4}{\sqrt t}.
$$

Rearranging,

$$
\boxed{t^{5/2}\geq c_3n^2,\qquad t\geq cn^{4/5}.}
$$

The whole [distinct-distance set](../../../../../distinct-distance-set.md) contains those distances from the selected point, proving the requested bound. The circular-arc method and the stronger one-point conclusion are due to [Székely](https://www.cs.tau.ac.il/~michas/szekely.pdf).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
