<h1 id="turan-graph">Turán graph</h1>

↑ **Parent:** [Turán's theorem](turan-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turán_graph)

The Turán graph $T_r(n)$ is a [complete multipartite graph](complete-multipartite-graph.md) with $r$ [independent sets](independent-set-graph-theory.md) of sizes differing by at most one, with every cross [edge](edge-of-a-graph.md) present. Empty parts are allowed when $r>n$.[third electronic edition (2005), §7.1, printed p. 165, definition of Turán graphs and convention for empty partition sets](graph-theory-by-reinhard-diestel.md)

<a id="image-the-turan-graph-t-3-8-has-three-independent-sets-of-sizes-3-3-2-giving-21-edges-and-no-four-vertex-clique"></a>
![](turan-balanced-tripartite-edge-count.png)

**[Figure 2](#image-the-turan-graph-t-3-8-has-three-independent-sets-of-sizes-3-3-2-giving-21-edges-and-no-four-vertex-clique). The Turán graph $T_3(8)$ has three independent sets of sizes $3,3,2$, giving $21$ edges and no four-vertex clique**.

In this example, the [independent sets](independent-set-graph-theory.md) are $A=\{a_1,a_2,a_3\}$, $B=\{b_1,b_2,b_3\}$ and $C=\{c_1,c_2\}$. Count the [edges](edge-of-a-graph.md) between each pair of parts:

$$
t_3(8)=3\cdot3+3\cdot2+3\cdot2=9+6+6=21.
$$

Any four [vertices](vertex-graph-theory.md) put at least two in the same [independent set](independent-set-graph-theory.md), by the [pigeonhole principle](pigeonhole-principle.md), so they cannot form $K_4$. Conversely, every choice of one [vertex](vertex-graph-theory.md) from each part is a [triangle in a graph](triangle-in-a-graph.md), giving $3\cdot3\cdot2=18$ [triangles in a graph](triangle-in-a-graph.md). [Clique](clique-graph-theory.md) exclusion here does not mean [triangle-free](triangle-free-graph.md).

For the exact count, [Euclidean division](euclidean-division.md) writes $n=rq+s$, where $q=\lfloor n/r\rfloor$ uses the [floor function](floor-function.md) and $s=n\bmod r$ is the [remainder](remainder.md), with $0\leq s<r$. There are $s$ parts of size $q+1$ and $r-s$ of size $q$. For any part sizes $a_1,\ldots,a_r$ summing to $n$, count cross [edges](edge-of-a-graph.md) by expanding the square:

$$
e(K_{a_1,\ldots,a_r})=\sum_{i<j}a_i a_j=\frac12\left(n^2-\sum_{i=1}^r a_i^2\right).
$$

Therefore

$$
t_r(n)=\frac12\left[n^2-s(q+1)^2-(r-s)q^2\right]
=\left(1-\frac1r\right)\frac{n^2}{2}-\frac{s(r-s)}{2r}.
$$

For $n=8,r=3$, we have $q=2,s=2$, giving $(64-2\cdot9-1\cdot4)/2=21$. The [Quadratic Turan edge bound](quadratic-turan-edge-bound.md) gives $64/3$ instead: the exact correction subtracts $1/3$.

Balancing is an [integer](integer-split.md) optimization with a simple reason. If two part sizes satisfy $a\geq b+2$, moving one [vertex](vertex-graph-theory.md) from the larger part to the smaller decreases their contribution to the [sum of squares](sum-of-squares.md) by

$$
a^2+b^2-(a-1)^2-(b+1)^2=2(a-b-1)>0,
$$

so it increases the [edge](edge-of-a-graph.md) count by $a-b-1$. For eight [vertices](vertex-graph-theory.md), parts $4,2,2$ give $20$ [edges](edge-of-a-graph.md); moving one [vertex](vertex-graph-theory.md) produces $3,3,2$ and $21$ [edges](edge-of-a-graph.md). The most symmetric permitted sizes pack the most cross [edges](edge-of-a-graph.md), which explains the sharp construction in [Turán's theorem](turan-s-theorem.md).

**Table of contents**

- [Triangle support line between bipartite and tripartite Turan graphs](triangle-support-line-between-bipartite-and-tripartite-turan-graphs.md)

## ↑ Ancestors (7)

1. [Turán's theorem](turan-s-theorem.md)
2. [Extremal graph theory](extremal-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Balancing a multipartite edge-triangle objective](balancing-a-multipartite-edge-triangle-objective.md)
- [Chromatic polynomial determines a Turán graph](chromatic-polynomial-determines-a-turan-graph.md)
- [Enumeration of subgraph-closed graph properties](enumeration-of-subgraph-closed-graph-properties.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/17f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/17g/i/solution.md)
- [Triangle support line between bipartite and tripartite Turan graphs](triangle-support-line-between-bipartite-and-tripartite-turan-graphs.md)
- [Turán graph](turan-graph.md)
- [Turán's theorem](turan-s-theorem.md)
