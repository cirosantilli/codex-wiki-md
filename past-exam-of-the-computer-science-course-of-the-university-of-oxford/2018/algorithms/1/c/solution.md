<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No.** In a [red-black tree](../../../../../red-black-tree.md) with no red nodes, equal [black height](../../../../../black-height.md) forces every [graph path](../../../../../path-in-a-graph.md) from the root to an absent-child position to have the same length. A real node cannot have exactly one real child: the two paths through that node would then have different numbers of black nodes. Recursively, every real level must be full. The tree is therefore a [perfect binary tree](../../../../../perfect-binary-tree.md).

With $h$ real levels its size is $1+2+\cdots+2^{h-1}=2^h-1$. A size of $23$ would require $2^h=24$, which is impossible for an [integer](../../../../../integer-split.md) $h$. The black null sentinels are not counted among the $23$ stored entries. This is the [all-black red-black tree size criterion](../../../../../all-black-red-black-tree-size-criterion.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
