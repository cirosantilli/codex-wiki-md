<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here each $T_i$ is a nonempty [connected subgraph of a tree](../../../../../connected-subgraph-of-a-tree.md), rather than a descendant-closed data-structure [subtree](../../../../../subtree.md). We prove the [Helly property for connected subgraphs of a tree](../../../../../helly-property-for-connected-subgraphs-of-a-tree.md) by [mathematical induction](../../../../../mathematical-induction.md) on the number of [vertices](../../../../../vertex-graph-theory.md) of $T$.

For a one-[vertex](../../../../../vertex-graph-theory.md) [tree](../../../../../tree-graph-theory-split.md), every nonempty $T_i$ contains that [vertex](../../../../../vertex-graph-theory.md). For a larger [tree](../../../../../tree-graph-theory-split.md), choose a [leaf of a tree](../../../../../leaf-of-a-tree.md) $v$ using part (i), and denote its unique neighbour by $w$. If some $T_i$ consists only of $v$, the assumed pairwise intersections force every $T_j$ to contain $v$, and we are done.

Otherwise, remove $v$ from every $T_i$ that contains it, leaving all other $T_i$ unchanged. Any affected $T_i$ has at least two [vertices](../../../../../vertex-graph-theory.md); connectedness forces it to contain $w$ and the [edge](../../../../../edge-of-a-graph.md) $vw$. Thus $v$ is a [leaf of a tree](../../../../../leaf-of-a-tree.md) of $T_i$, and part (ii) shows that its deletion leaves a nonempty [tree](../../../../../tree-graph-theory-split.md). All reduced $T_i$ are therefore nonempty [connected subgraphs of a tree](../../../../../connected-subgraph-of-a-tree.md) $T\setminus v$.

They still intersect pairwise. An original common [vertex](../../../../../vertex-graph-theory.md) other than $v$ survives. If a pair had only $v$ in common, both members would also contain $w$, by the previous paragraph, contradicting that it was their only common [vertex](../../../../../vertex-graph-theory.md). The induction hypothesis now supplies a common [vertex](../../../../../vertex-graph-theory.md) of the reduced family, which is also common to the original family. Consequently

$$
\boxed{\bigcap_{i=1}^kV(T_i)\ne\varnothing.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
