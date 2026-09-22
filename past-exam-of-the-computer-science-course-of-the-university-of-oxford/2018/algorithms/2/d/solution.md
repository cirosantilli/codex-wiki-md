<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In [depth-first search](../../../../../depth-first-search.md) of an [undirected graph](../../../../../undirected-graph.md), every [edge](../../../../../edge-of-a-graph.md) joins a [vertex](../../../../../vertex-graph-theory.md) to one of its ancestors or descendants in the discovery [tree](../../../../../tree-graph-theory-split.md). To see this directly, suppose $u$ is discovered before its neighbour $v$. If $v$ is still undiscovered, the search from $u$ cannot finish before discovering $v$: it eventually scans $uv$. Thus $v$ is discovered while the call for $u$ remains active and belongs to its descendant [subtree](../../../../../subtree.md).[Chapter 6, §6.1: active recursion intervals, tree/back edges and ancestor relations](../../../../../depth-first-search-by-jeff-erickson.md)

For any [edge](../../../../../edge-of-a-graph.md) $uv$, its ancestor endpoint therefore has a proper descendant and hence at least one child. It is an [internal vertex of a rooted tree](../../../../../internal-vertex-of-a-rooted-tree.md). **Every [edge](../../../../../edge-of-a-graph.md) has an internal endpoint**, so the internal [vertices](../../../../../vertex-graph-theory.md) form a [vertex cover](../../../../../vertex-cover.md). The relevant [leaves of a rooted tree](../../../../../leaf-of-a-rooted-tree.md) here have no children in the rooted discovery [tree](../../../../../tree-graph-theory-split.md); a root of [vertex degree](../../../../../degree-graph-theory.md) one can still be internal.

## ↑ Ancestors (11)

1. [D](../d.md)
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
