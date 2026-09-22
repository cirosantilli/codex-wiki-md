<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Root the [tree](../../../../../tree-graph-theory-split.md) arbitrarily. For each [vertex](../../../../../vertex-graph-theory.md) $v$, let $D_1(v)$ be the minimum [vertex cover](../../../../../vertex-cover.md) size in its descendant [subtree](../../../../../subtree.md), conditional on selecting $v$, and $D_0(v)$ the corresponding minimum conditional on omitting $v$. Process the [vertices](../../../../../vertex-graph-theory.md) in [postorder traversal](../../../../../postorder-traversal.md). For every child $u$ of $v$,

$$
\boxed{D_1(v)=1+\sum_{u\text{ child of }v}\min\{D_0(u),D_1(u)\},\qquad D_0(v)=\sum_{u\text{ child of }v}D_1(u).}
$$

At a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md), the empty [sums](../../../../../sum.md) give $D_1=1,D_0=0$. Return **$\min\{D_0(r),D_1(r)\}$** at the root $r$.

For [algorithm correctness](../../../../../algorithm-correctness.md), if $v$ is selected, each child [subtree](../../../../../subtree.md) may independently use its cheaper state, since the connecting [edge](../../../../../edge-of-a-graph.md) is already covered by $v$. If $v$ is omitted, each child must be selected to cover its connecting [edge](../../../../../edge-of-a-graph.md). Distinct child [subtrees](../../../../../subtree.md) have no [edges](../../../../../edge-of-a-graph.md) between them because the input is a [tree](../../../../../tree-graph-theory-split.md). These observations prove the recurrences by [structural induction](../../../../../structural-induction.md). Each [edge](../../../../../edge-of-a-graph.md) contributes constant work once, giving **$O(|V|)$ [time complexity](../../../../../time-complexity.md) and $O(|V|)$ space** with [adjacency lists](../../../../../adjacency-list.md). The single-vertex [tree](../../../../../tree-graph-theory-split.md) correctly has optimum zero. This is [minimum vertex cover of a tree](../../../../../minimum-vertex-cover-of-a-tree.md) by [dynamic programming](../../../../../dynamic-programming.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
