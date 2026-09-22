<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use fan-out four to mean at most four child pointers per internal node. A height increase requires a [B+ tree node split](../../../../../b-plus-tree-node-split.md) at the root. Immediately after that [B+ tree node split](../../../../../b-plus-tree-node-split.md), the new root has exactly two children.

One further insertion follows one search path. Any chain of [B+ tree node splits](../../../../../b-plus-tree-node-split.md) along that path can pass at most one additional separator and child pointer to the root. Its number of children therefore rises from two to at most three, below the maximum four. Thus

$$
\boxed{\text{No: two consecutive insertions cannot both increase the height.}}
$$

The argument includes an initially leaf-only [B+ tree](../../../../../b-plus-tree.md): its first root split likewise creates a root with two children. Even if the next insertion causes a child split immediately, the new root still has room. The conclusion assumes the standard insertion operation with one overflowing node split into two; it does not depend on whether height counts edges or levels.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
