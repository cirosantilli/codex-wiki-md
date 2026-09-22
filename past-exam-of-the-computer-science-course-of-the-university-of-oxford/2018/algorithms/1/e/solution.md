<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $y=x+1$. After [splaying](../../../../../splaying.md) on $x$, that key is at the root, and $y$ is the smallest key in its right [subtree](../../../../../subtree.md). This uses the [integer](../../../../../integer-split.md) assumption: no stored key lies strictly between $x$ and $y$. Thus $y$ has an empty left [subtree](../../../../../subtree.md) while it remains within the right [subtree](../../../../../subtree.md) of $x$.

Now perform ordinary bottom-up [splaying](../../../../../splaying.md) on $y$. Until the final step involving $x$, all [tree rotations](../../../../../tree-rotation.md) occur below $x$ and leave it at the root. There are only two possible final cases.

- If $y$ is the right child of $x$, a single [zig step](../../../../../zig-step.md) rotates $y$ above $x$, placing $x$ immediately to its left.
- Otherwise $y$ is a grandchild of $x$. Its parent $p$ lies in the right [subtree](../../../../../subtree.md) of $x$ and must satisfy $p>y$. Hence the last two directions are right then left. A [zig-zag step](../../../../../zig-zag-step.md) rotates $y$ above $p$ and then above $x$, again placing $x$ immediately to its left. A right-right final configuration is impossible because $y$ is the minimum of this [subtree](../../../../../subtree.md).

Therefore **$x$ becomes the left child of $x+1$**. The argument applies more generally to [consecutive keys in a binary search tree](../../../../../consecutive-keys-in-a-binary-search-tree.md), even when their numerical difference is not one.

## ↑ Ancestors (11)

1. [E](../e.md)
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
