# Chromatic index

↑ **Parent:** [Edge coloring](edge-coloring.md)

The [chromatic index](chromatic-index.md) $\chi\prime(G)$, also called the [edge chromatic number](edge-chromatic-number.md), is the least number of labels in a [proper edge colouring](proper-edge-coloring.md) of a finite [undirected graph](undirected-graph.md) without [self-loops](loop-graph-theory.md). Equivalently, it is the smallest number of [matchings in a graph](matching-graph-theory.md) whose [set partition](set-partition.md) covers all the [edges](edge-of-a-graph.md). We take $\chi\prime(G)=0$ when there are no [edges](edge-of-a-graph.md). For an arbitrary [edge colouring](edge-coloring.md), one colour always suffices whenever an [edge](edge-of-a-graph.md) exists, so properness is essential to this definition. The [chromatic number](chromatic-number.md) $\chi(G)$ instead colours [vertices](vertex-graph-theory.md).[Colouring, author-hosted chapter preview, p. 124: chromatic index and line graph](graph-theory-by-reinhard-diestel.md)

To establish an exact [chromatic index](chromatic-index.md), supply both a [proper edge colouring](proper-edge-coloring.md) and a reason that fewer colours cannot work. Every [edge](edge-of-a-graph.md) at a fixed [vertex](vertex-graph-theory.md) must have its own colour, giving the lower bound $\chi\prime(G)\geq\Delta(G)$, where $\Delta(G)$ is the [maximum degree of a graph](maximum-degree-of-a-graph.md). The bound need not be attained: it counts a single resource's workload, while conflicts can also accumulate around a [graph cycle](cycle-in-a-graph.md).

<a id="image-worked-proper-edge-colourings-a-triangle-in-a-graph-needs-three-colours-while-an-even-cycle-graph-needs-two"></a>
![](edge-coloring-triangle-even-cycle.png)

**[Figure 18](#image-worked-proper-edge-colourings-a-triangle-in-a-graph-needs-three-colours-while-an-even-cycle-graph-needs-two). Worked proper edge colourings: a triangle in a graph needs three colours, while an even cycle graph needs two**. Numbers beside [edges](edge-of-a-graph.md) are colour labels; letters at dots are [vertices](vertex-graph-theory.md). Both [graphs](graph-split.md) have [maximum degree of a graph](maximum-degree-of-a-graph.md) two. The [triangle in a graph](triangle-in-a-graph.md) has three pairwise conflicting [edges](edge-of-a-graph.md), while opposite [edges](edge-of-a-graph.md) of the square can share a colour.

For the [triangle in a graph](triangle-in-a-graph.md) $K_3$ with [edges](edge-of-a-graph.md) $ab,bc,ca$, every pair of [edges](edge-of-a-graph.md) shares a [vertex](vertex-graph-theory.md), so all three require different labels. The assignment $c(ab)=1,c(bc)=2,c(ca)=3$ works, proving $\chi\prime(K_3)=3$ although $\Delta(K_3)=2$. In its [line graph](line-graph.md), those three [edges](edge-of-a-graph.md) become a three-[vertex](vertex-graph-theory.md) [clique](clique-graph-theory.md). Treating this as three pair-resource jobs makes the obstruction tangible: each resource has only two jobs, but every pair of jobs conflicts, so no slot can contain two jobs.

For the square [cycle graph](cycle-graph.md) $C_4$ with [edges](edge-of-a-graph.md) $ab,bc,cd,da$, use $c(ab)=c(cd)=1$ and $c(bc)=c(da)=2$. Each [colour class](colour-class.md) is a [matching in a graph](matching-graph-theory.md), and each [vertex](vertex-graph-theory.md) has one [edge](edge-of-a-graph.md) of each colour. Since $\Delta(C_4)=2$, this proves $\chi\prime(C_4)=2$. More generally, alternation closes on any even [cycle graph](cycle-graph.md) $C_{2m}$, $m\geq2$. On an [odd cycle](odd-cycle.md) $C_{2m+1}$, $m\geq1$, two-colour alternation would make the last and first [edges](edge-of-a-graph.md) share a colour at their common [vertex](vertex-graph-theory.md); a third colour on the last [edge](edge-of-a-graph.md) suffices. Thus even [cycle graphs](cycle-graph.md) have [chromatic index](chromatic-index.md) two and odd [cycle graphs](cycle-graph.md) have [chromatic index](chromatic-index.md) three. These exact examples show why [maximum degree of a graph](maximum-degree-of-a-graph.md) alone does not determine the answer.

**Table of contents**

- [Chromatic index bounds](chromatic-index-bounds.md)

## ↑ Ancestors (7)

1. [Edge coloring](edge-coloring.md)
2. [Graph coloring](graph-coloring.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Chromatic index](chromatic-index.md)
- [Edge coloring as scheduling](edge-coloring-as-scheduling.md)
- [Galvin theorem for bipartite list edge coloring](galvin-theorem-for-bipartite-list-edge-coloring.md)
- [List-chromatic index](list-chromatic-index.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/2/solution.md)
