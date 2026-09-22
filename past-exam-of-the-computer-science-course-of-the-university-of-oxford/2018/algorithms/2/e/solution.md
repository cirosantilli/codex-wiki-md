<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

We construct an [injection](../../../../../injective-function.md) from the [unmatched vertices in a matching](../../../../../unmatched-vertex-in-a-matching.md) to the [leaves of a rooted tree](../../../../../leaf-of-a-rooted-tree.md). Start a downward [graph path](../../../../../path-in-a-graph.md) at each unmatched [vertex](../../../../../vertex-graph-theory.md) $u$. If the current [vertex](../../../../../vertex-graph-theory.md) is a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md), stop. Otherwise choose any child $v$. The current [vertex](../../../../../vertex-graph-theory.md) is either the unmatched starting point or a [vertex](../../../../../vertex-graph-theory.md) already matched to its own parent.

In either case, $v$ cannot be unmatched: the [proper matching in a rooted tree](../../../../../proper-matching-in-a-rooted-tree.md) condition would require its parent to be matched to one of $v$'s [siblings in a rooted tree](../../../../../sibling-in-a-rooted-tree.md), whereas that parent is either unmatched or already matched upward. Nor can $v$ be matched to its parent. Its matching partner must therefore be one of its own children, say $w$. Extend the [graph path](../../../../../path-in-a-graph.md) by the two [edges](../../../../../edge-of-a-graph.md) to $v$ and then to $w$, and continue from $w$.

Every extension descends two levels, so finiteness guarantees termination at a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md). Every visited [vertex](../../../../../vertex-graph-theory.md) except the starting point is matched. The constructed [graph paths](../../../../../path-in-a-graph.md) for different unmatched starting points are disjoint: if two downward [graph paths](../../../../../path-in-a-graph.md) in a [tree](../../../../../tree-graph-theory-split.md) meet, one starting point must lie on the other path, which would put a second unmatched [vertex](../../../../../vertex-graph-theory.md) after the first. That is impossible. Hence their terminal [leaves of a rooted tree](../../../../../leaf-of-a-rooted-tree.md) are distinct, proving

$$
\boxed{|U(M)|\leq|L(T)|.}
$$

Only the properness condition for unmatched non-root [vertices](../../../../../vertex-graph-theory.md) was used. If the root is unmatched and the convention exempts it because it has no parent, the same construction starts there and still works. Thus the root convention does not affect the claimed inequality. This proves the [unmatched-vertex bound for a proper tree matching](../../../../../unmatched-vertex-bound-for-a-proper-tree-matching.md) without requiring $M$ to have maximum size.

## ↑ Ancestors (11)

1. [E](../e.md)
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
