<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the usual bottom-up [splaying](../../../../../splaying.md) operations. We prove the stronger result that **at most three successful calls suffice**. No insertions or deletions are needed.

If the chosen key $x$ is the minimum stored key, first perform [splaying](../../../../../splaying.md) on $x$ and then on its immediate successor. The argument for [consecutive keys in a binary search tree](../../../../../consecutive-keys-in-a-binary-search-tree.md) makes $x$ the left child of the successor with an empty right [subtree](../../../../../subtree.md); minimality makes its left [subtree](../../../../../subtree.md) empty too. Hence $x$ is a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md). The maximum-key case is the mirror image.

Suppose $x$ is an interior key. Since at least four keys are stored, there are either two keys larger than $x$ or two smaller than $x$. In the former case choose four consecutive stored keys

$$
a<x<b<c,
$$

where $a$ is the predecessor of $x$, and $b,c$ are the next two successors. Perform **$\operatorname{Splay}(c),\operatorname{Splay}(a),\operatorname{Splay}(b)$**.

Here is a complete check of the local shapes. After the first call, $c$ is the root. After the second, $a$ is the root; every key below $a$ is in its left [subtree](../../../../../subtree.md) $A$, and every key above $c$ stays in the right [subtree](../../../../../subtree.md) $D$ of $c$. These outside [subtrees](../../../../../subtree.md) cannot interfere with the next search. Between $a$ and $c$ there are only $x,b$. The last step of [splaying](../../../../../splaying.md) on $a$ is either a [zig step](../../../../../zig-step.md), leaving $c$ as its right child; a [zig-zag step](../../../../../zig-zag-step.md), with the same result; or a [zig-zig step](../../../../../zig-zig-step.md), leaving some $p\in\{x,b\}$ as its right child with $c$ immediately to the right of $p$. Consequently the possible right [subtrees](../../../../../subtree.md) of $a$ are exactly among these four forms, using $k(L,R)$ for a node with its left and right [subtrees](../../../../../subtree.md):

$$
\begin{array}{c|c}
\text{right subtree of }a\text{ after the second call}&\text{shape after splaying }b\\\hline
c\bigl(b(x,\varnothing),D\bigr)&b\bigl(a(A,x),c(\varnothing,D)\bigr)\\
c\bigl(x(\varnothing,b),D\bigr)&b\bigl(a(A,x),c(\varnothing,D)\bigr)\\
b\bigl(x,c(\varnothing,D)\bigr)&b\bigl(a(A,x),c(\varnothing,D)\bigr)\\
x\bigl(\varnothing,c(b,D)\bigr)&b\bigl(a(A,x),c(\varnothing,D)\bigr)
\end{array}
$$

Here an unexpanded $x$ or $b$ denotes a node with no children. Each row follows by the indicated one or two [tree rotations](../../../../../tree-rotation.md) in each bottom-up step. All rows end with $x$ as the right child of $a$, with both its [subtrees](../../../../../subtree.md) empty. If instead two keys below $x$ are available, reflect the construction, exchanging left and right and reversing the order of keys. This proves [splaying a chosen node into a leaf](../../../../../splaying-a-chosen-node-into-a-leaf.md) for every node of every [splay tree](../../../../../splay-tree.md) of size at least four.

## ↑ Ancestors (11)

1. [F](../f.md)
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
