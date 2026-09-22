# Binary tree

↑ **Parent:** [Data structure](data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_tree)

A [binary tree](binary-tree.md), in the [data structure](data-structure.md) convention used here, is a [rooted tree](rooted-tree.md) in which each [vertex](vertex-graph-theory.md) has zero, one or two [children in a rooted tree](child-in-a-rooted-tree.md), occupying distinct left and right positions. A single left child and a single right child give different [binary trees](binary-tree.md). A [vertex](vertex-graph-theory.md) with no [children in a rooted tree](child-in-a-rooted-tree.md) is called a leaf. An empty [binary tree](binary-tree.md) has no [root of a tree](root-of-a-tree.md) and is also allowed as a storage case. [Pat Morin, Open Data Structures, chapter 6: roots, left and right children](https://opendatastructures.org/newhtml/ods/latex2/binarytrees.html)

For example, give the [root of a tree](root-of-a-tree.md) label $4$, its left child label $2$ and its right child label $6$. Attach $1,3$ as the left and right [children in a rooted tree](child-in-a-rooted-tree.md) of $2$, and $5,7$ as those of $6$. This [binary tree](binary-tree.md) has seven [vertices](vertex-graph-theory.md), six [edges](edge-of-a-graph.md), and [height of a binary tree](height-of-a-binary-tree.md) $2$: a longest downward [graph path](path-in-a-graph.md) contains two [edges](edge-of-a-graph.md). The first diagram below shows this shape alongside the [binary tree](binary-tree.md) consisting only of successive right children $1,2,\ldots,7$, whose [height of a binary tree](height-of-a-binary-tree.md) is $6$.

Left and right positions specify an ordered shape, not a numerical [total order](total-order.md) on stored labels. Swapping labels $1$ and $7$ in the first example still gives a [binary tree](binary-tree.md), but destroys the [binary search tree](binary-search-tree.md) property. Nor must a [binary tree](binary-tree.md) be balanced: the right-child chain is just as valid. The same shape convention supports a [binary heap](binary-heap.md), a [Huffman code](huffman-code.md), or a [binary search tree](binary-search-tree.md), each with its own additional rules. The useful idea is to describe two smaller [subtrees](subtree.md) at each [vertex](vertex-graph-theory.md), making [structural recursion](structural-recursion.md) natural.

**Table of contents**

- [Subtree](subtree.md)
- [Height of a binary tree](height-of-a-binary-tree.md)
- [Inorder traversal](inorder-traversal.md)
- [Binary search tree](binary-search-tree.md)
  - [Dictionary intersection](dictionary-intersection.md)
- [Complete binary tree](complete-binary-tree.md)
- [Full binary tree](full-binary-tree.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Binary search tree](binary-search-tree.md)
- [Binary tree](binary-tree.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Comparison sorting lower bound](comparison-sorting-lower-bound.md)
- [Complete binary tree](complete-binary-tree.md)
- [Height of a binary tree](height-of-a-binary-tree.md)
- [Huffman code](huffman-code.md)
- [Huffman coding](huffman-coding.md)
- [Inorder traversal](inorder-traversal.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/5/a/ii/solution.md)
- [Rooted tree](rooted-tree.md)
- [Subtree](subtree.md)
- [Ultrametric space](ultrametric-space.md)
