<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose a root. For each vertex $v$, define $I(v)$ as the maximum size in its descendant [subtree](../../../../../subtree.md) when $v$ is included, and $O(v)$ as that size when $v$ is excluded. For its children $w$,

$$
\boxed{I(v)=1+\sum_{w}O(w),\qquad
O(v)=\sum_w\max\{I(w),O(w)\}.}
$$

A leaf has $I=1,O=0$. If $v$ is included, all its children must be excluded. If $v$ is excluded, either child state is allowed. Different child subtrees have no edges between them because the graph is a [tree](../../../../../tree-graph-theory-split.md), so their contributions can be optimized independently. This proves the recurrence by [structural induction](../../../../../structural-induction.md).

Evaluate the two states in [postorder traversal](../../../../../postorder-traversal.md). At root $r$, the answer is $\max\{I(r),O(r)\}$. For reconstruction, pick an attaining root state; an included vertex forces every child to its excluded state, while an excluded vertex permits each child to choose its larger state. Record the included vertices during this second traversal, breaking ties consistently.

With [adjacency lists](../../../../../adjacency-list.md), rooting, state evaluation and reconstruction each take **$O(|V|+|E|)=O(n)$ time**, with $O(n)$ stored states and output. This is [maximum independent set in a tree](../../../../../maximum-independent-set-in-a-tree.md).

The source describes an [independent set](../../../../../independent-set-graph-theory.md) as a proper subset. For a tree with at least one edge, every independent set is automatically proper, so the algorithm meets that convention. If it is enforced literally for the single-vertex tree, return the empty set of size zero there; the usual non-strict subset convention would instead return its one vertex.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
