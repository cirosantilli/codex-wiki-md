<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ramsey number](../../../../../ramsey-number.md) $R(s,t)$ is the least [integer](../../../../../integer-split.md) $N$ such that every [graph](../../../../../graph-split.md) on $N$ [vertices](../../../../../vertex-graph-theory.md) contains either a [clique](../../../../../clique-graph-theory.md) of size $s$ or an [independent set](../../../../../independent-set-graph-theory.md) of size $t$. Equivalently, every red-blue [colouring](../../../../../colouring-of-a-set.md) of the [edges](../../../../../edge-of-a-graph.md) of $K_N$ contains a red $K_s$ or a blue $K_t$.

Put $a=R(s-1,t)$, $b=R(s,t-1)$ and consider a [graph](../../../../../graph-split.md) on $a+b$ [vertices](../../../../../vertex-graph-theory.md). Fix a [vertex](../../../../../vertex-graph-theory.md) $v$. If it has at least $a$ [neighbours](../../../../../neighbour-of-a-vertex.md), their induced [graph](../../../../../graph-split.md) contains either a [clique](../../../../../clique-graph-theory.md) of size $s-1$, which together with $v$ gives a [clique](../../../../../clique-graph-theory.md) of size $s$, or an [independent set](../../../../../independent-set-graph-theory.md) of size $t$. Otherwise $v$ has at least $b$ nonneighbours. Their induced [graph](../../../../../graph-split.md) contains either a [clique](../../../../../clique-graph-theory.md) of size $s$, or an [independent set](../../../../../independent-set-graph-theory.md) of size $t-1$, which can be enlarged by $v$. Thus

$$
\boxed{R(s,t)\leq R(s-1,t)+R(s,t-1).}
$$

Since $R(2,3)=R(3,2)=3$, this gives $R(3,3)\leq6$. For the reverse bound, the [five-cycle](../../../../../cycle-graph.md) has no [triangle](../../../../../triangle-in-a-graph.md) and no [independent set](../../../../../independent-set-graph-theory.md) of size three: its [complement](../../../../../complement-of-a-set.md) is again a [five-cycle](../../../../../cycle-graph.md), so it too is triangle-free. Hence the property fails on five [vertices](../../../../../vertex-graph-theory.md) and

$$
\boxed{R(3,3)=6.}
$$

<a id="a/1/a/image-the-five-cycle-and-its-complement-witness-the-lower-bound-for-r-3-3"></a>
![](../../../../../past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011-ramsey-five-cycle.png)

**[Figure 1](#a/1/a/image-the-five-cycle-and-its-complement-witness-the-lower-bound-for-r-3-3). The five-cycle and its complement witness the lower bound for R(3,3)** Both panels use the same five labelled vertices. The red cycle and the blue complementary edges are each triangle-free; crossings in the right panel are not vertices.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
