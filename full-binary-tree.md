# Full binary tree

↑ **Parent:** [Binary tree](binary-tree.md)

A [full binary tree](full-binary-tree.md) is a [binary tree](binary-tree.md) in which every nonleaf has exactly two [children in a rooted tree](child-in-a-rooted-tree.md); equivalently, no [vertex](vertex-graph-theory.md) has just one child.[Data Structures and Algorithms, section 9.1.1: full shape and Huffman coding tree example](data-structures-and-algorithms-edited-by-peter-ljunglof-and-others/9-1-binary-trees.md)

A binary [Huffman code](huffman-code.md) with at least two positive-probability symbols has a full code [tree](tree-graph-theory-split.md): a [vertex](vertex-graph-theory.md) with only one child could be suppressed to shorten all codewords below it.

Let $A$ have [children in a rooted tree](child-in-a-rooted-tree.md) $B,C$, and let $C$ have [children in a rooted tree](child-in-a-rooted-tree.md) $D,E$, with $B,D,E$ leaves. Every [vertex](vertex-graph-theory.md) has zero or two [children in a rooted tree](child-in-a-rooted-tree.md), so this five-[vertex](vertex-graph-theory.md) [binary tree](binary-tree.md) is full. It is not a [complete binary tree](complete-binary-tree.md): level $2$ has empty positions under $B$ before the occupied positions under $C$. Instead put $D,E$ under $B$ and leave $C$ a leaf. The resulting five-[vertex](vertex-graph-theory.md) [binary tree](binary-tree.md) is both full and complete, yet is not a [perfect binary tree](perfect-binary-tree.md) because its leaves occur at two different distances from the [root of a tree](root-of-a-tree.md).

If a nonempty finite [full binary tree](full-binary-tree.md) has $i$ nonleaf [vertices](vertex-graph-theory.md) and $\ell$ leaves, then its [edges](edge-of-a-graph.md) can be counted as $2i$, two leaving each nonleaf, or as $i+\ell-1$, using the [tree](tree-graph-theory-split.md) count. Hence

$$
\ell=i+1,\qquad n=i+\ell=2i+1.
$$

Thus $n$ is odd, but odd size alone does not imply fullness: a three-[vertex](vertex-graph-theory.md) chain is a counterexample. Nor does fullness guarantee small [height of a binary tree](height-of-a-binary-tree.md). Repeatedly give one continuing [vertex](vertex-graph-theory.md) a leaf in one slot and another continuing [vertex](vertex-graph-theory.md) in the other, ending with two leaves. With $i\geq1$ nonleaf [vertices](vertex-graph-theory.md), this constructs a [full binary tree](full-binary-tree.md) of $n=2i+1$ [vertices](vertex-graph-theory.md) and [height of a binary tree](height-of-a-binary-tree.md) $i$. The two-children rule permits height growing linearly with size.

## ↑ Ancestors (4)

1. [Binary tree](binary-tree.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Binary parenthesization](binary-parenthesization.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Complete binary tree](complete-binary-tree.md)
- [Full binary tree](full-binary-tree.md)
- [Huffman sibling property](huffman-sibling-property.md)
- [Nonunique optimal prefix code](nonunique-optimal-prefix-code.md)
- [Optimal prefix code](optimal-prefix-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/1/e/solution.md)
- [Perfect binary tree](perfect-binary-tree.md)
