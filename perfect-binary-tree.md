# Perfect binary tree

↑ **Parent:** [Binary tree](binary-tree.md)

A nonempty [binary tree](binary-tree.md) in which every level, including the deepest, contains all its possible [vertices](vertex-graph-theory.md). Equivalently, it is a [full binary tree](full-binary-tree.md) whose leaves are all at the same [graph distance](distance-graph-theory.md) from the [root of a tree](root-of-a-tree.md).[Data Structures and Algorithms, section 9.1.1: perfect shape, equal leaf levels, and Figure 9.4](data-structures-and-algorithms-edited-by-peter-ljunglof-and-others/9-1-binary-trees.md)

Every [perfect binary tree](perfect-binary-tree.md) is both a [full binary tree](full-binary-tree.md) and a [complete binary tree](complete-binary-tree.md); the five-[vertex](vertex-graph-theory.md) example above shows that the converse fails even when both properties hold. These definitions fix the terminology used here.

For [height of a binary tree](height-of-a-binary-tree.md) $h\geq0$, the level sizes are $1,2,4,\ldots,2^h$, giving $n=2^{h+1}-1$ by a [geometric series](geometric-series.md). There are $2^h$ leaves. The seven-[vertex](vertex-graph-theory.md) example has level sizes $1,2,4$ and [height of a binary tree](height-of-a-binary-tree.md) $2$; the single-[vertex](vertex-graph-theory.md) [binary tree](binary-tree.md) is already perfect, with $h=0$. More generally, joining two [perfect binary trees](perfect-binary-tree.md) of equal [height of a binary tree](height-of-a-binary-tree.md) under a fresh [root of a tree](root-of-a-tree.md) gives the next such shape. Equal heights are essential: fullness alone allows unequal leaf distances. A [perfect binary tree](perfect-binary-tree.md) realizes the maximum number of [vertices](vertex-graph-theory.md) for its [height of a binary tree](height-of-a-binary-tree.md), making the exponential capacity behind short lookup [graph paths](path-in-a-graph.md) visible.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (4)

1. [Binary tree](binary-tree.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Complete binary tree](complete-binary-tree.md)
- [Full binary tree](full-binary-tree.md)
- [Height of a binary tree](height-of-a-binary-tree.md)
- [Perfect binary tree](perfect-binary-tree.md)
