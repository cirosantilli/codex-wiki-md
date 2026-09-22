# Height of a binary tree

↑ **Parent:** [Binary tree](binary-tree.md)

For a nonempty [binary tree](binary-tree.md), the largest number of [edges](edge-of-a-graph.md) on a downward [graph path](path-in-a-graph.md) from its [root of a tree](root-of-a-tree.md) to a leaf. A single [vertex](vertex-graph-theory.md) has [height of a binary tree](height-of-a-binary-tree.md) $0$; a chain of $n\geq1$ [vertices](vertex-graph-theory.md) has [height of a binary tree](height-of-a-binary-tree.md) $n-1$. A convenient [recursion](recursion-computer-science.md) convention assigns an empty [binary tree](binary-tree.md) height $-1$, giving $h=1+\max(h_L,h_R)$ for the left and right [subtrees](subtree.md). A [binary search tree](binary-search-tree.md) lookup visits at most $h+1$ [vertices](vertex-graph-theory.md).

The convention counts [edges](edge-of-a-graph.md), rather than [vertices](vertex-graph-theory.md) on the longest [graph path](path-in-a-graph.md). Its recursive form is

$$
h(\varnothing)=-1,\qquad h(T)=1+\max\{h(L),h(R)\}\quad(T\ne\varnothing).
$$

[Data Structures and Algorithms, section 9.1.2, height pseudocode: null returns -1](data-structures-and-algorithms-edited-by-peter-ljunglof-and-others/9-1-binary-trees.md)

For a leaf, both [subtrees](subtree.md) are empty, giving $1+\max(-1,-1)=0$. For the mixed four-[vertex](vertex-graph-theory.md) example, $h(C)=h(D)=0$, $h(B)=1+\max(-1,0)=1$, and $h(A)=1+\max(1,0)=2$. The four-[vertex](vertex-graph-theory.md) chain has [height of a binary tree](height-of-a-binary-tree.md) $3$. A convention that counts [vertices](vertex-graph-theory.md) would add one to every nonempty [binary tree](binary-tree.md) height, so a height formula must specify its convention.

At distance $d$ from the [root of a tree](root-of-a-tree.md), there are at most $2^d$ [vertices](vertex-graph-theory.md): each [vertex](vertex-graph-theory.md) in the preceding level has at most two [children in a rooted tree](child-in-a-rooted-tree.md). Summing this [geometric series](geometric-series.md) and using the longest [graph path](path-in-a-graph.md) gives, for $n\geq1$,

$$
n\leq2^{h+1}-1,\qquad \lceil\log_2(n+1)\rceil-1\leq h\leq n-1.
$$

The upper bound is attained by a chain; a [perfect binary tree](perfect-binary-tree.md) attains the capacity bound. For $n=4$, the minimum possible [height of a binary tree](height-of-a-binary-tree.md) is $\lceil\log_2 5\rceil-1=2$, as in the mixed example, while the maximum is $3$. The [binary tree](binary-tree.md) definition permits both extremes. Small [height of a binary tree](height-of-a-binary-tree.md) bounds the length of a directed lookup in a [binary search tree](binary-search-tree.md); evaluating the [height of a binary tree](height-of-a-binary-tree.md) by the displayed [structural recursion](structural-recursion.md) still examines all $n$ [vertices](vertex-graph-theory.md), requiring $O(n)$ [time complexity](time-complexity.md) under constant-cost child access and arithmetic.

## ↑ Ancestors (4)

1. [Binary tree](binary-tree.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Binary search tree](binary-search-tree.md)
- [Binary tree](binary-tree.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Bounding volume hierarchy traversal](bounding-volume-hierarchy-traversal.md)
- [Complete binary tree](complete-binary-tree.md)
- [Full binary tree](full-binary-tree.md)
- [Height of a binary tree](height-of-a-binary-tree.md)
- [Perfect binary tree](perfect-binary-tree.md)
