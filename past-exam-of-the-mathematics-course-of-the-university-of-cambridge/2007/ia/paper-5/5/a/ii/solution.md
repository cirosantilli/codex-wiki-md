<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a finite [binary tree](../../../../../../../binary-tree.md), `gordon p t` expresses **the existence of a root-to-`Lf` path on which every branch-node label satisfies `p`**. The empty tree has a length-zero path and returns `true`. At `Br(x,left,right)`, such a path exists precisely when `p x` holds and at least one child admits such a path. This is the recursive Boolean equation derived in part (i).

The property is neither “all labels in the tree satisfy `p`” nor “some label satisfies `p`”. A bad label in an unchosen subtree does not prevent success, but a bad root label prevents every root-to-leaf path. The traversal performs a left-first search for a qualifying path.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
