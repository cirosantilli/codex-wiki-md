<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An individual can have any number of children, so use a [rose tree](../../../../../rose-tree.md), with one [list](../../../../../list-abstract-data-type.md) of child [trees](../../../../../tree-graph-theory-split.md) at each root:

```
data DescendantTree = Desc Person [DescendantTree]
  deriving Show

descendants :: Database -> Person -> DescendantTree
descendants db p = Desc p (map (descendants db) (children db p))
```

The root records `p`, its immediate child [trees](../../../../../tree-graph-theory-split.md) record `children db p`, and [recursion](../../../../../recursion-computer-science.md) repeats the same construction at each generation. An individual with no recorded children produces `Desc p []`. For a finite [database](../../../../../database.md) whose parent-child [directed graph](../../../../../directed-graph.md) is [acyclic](../../../../../forest.md), every recursive descent advances along a path that cannot revisit a vertex, so the construction terminates. On inconsistent cyclic records it can unfold indefinitely; finiteness of the [database](../../../../../database.md) alone is insufficient for termination.

Two branches may contain the same descendant, as happens when relatives have a child. This is appropriate for the requested [tree](../../../../../tree-graph-theory-split.md) unfolding; it preserves both lines of descent rather than silently choosing one. The concise constructor equation is

$$
\boxed{D(p)=\mathrm{Desc}\ p\ [D(c)\mid c\in\operatorname{children}(db,p)].}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
