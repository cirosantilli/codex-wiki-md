<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Suppose a leaf has depth $t\le s-2$. By part a there is a sibling pair of leaves at depth $s$. These leaves are disjoint from the shallow leaf and its descendants, since a leaf has no descendants. Modify the [prefix tree of a code](../../../../../../prefix-tree-of-a-code.md) by splitting the shallow leaf into two leaves at depth $t+1$ and replacing the deepest sibling pair by their parent as one leaf at depth $s-1$. The number of leaves remains $m$, so assign the equiprobable source letters bijectively to the new leaves.

The sum of depths for the three affected leaves changes from $t+2s$ to $2(t+1)+(s-1)$. The change is

$$
2(t+1)+(s-1)-(t+2s)=t-s+1\le-1.
$$

All other depths are unchanged. Since probabilities are equal, this strictly decreases the [expected codeword length](../../../../../../expected-codeword-length.md), contradicting the optimality of the [Huffman code](../../../../../../huffman-code.md). This is the [balancing exchange for a uniform optimal prefix code](../../../../../../balancing-exchange-for-a-uniform-optimal-prefix-code.md). There is therefore no leaf of depth at most $s-2$, proving

$$
\boxed{s_i\in\{s-1,s\}\text{ for every }i,\qquad n_{s-1}+n_s=m.}
$$

The argument applies to every optimal binary prefix tree for the uniform source, independently of how Huffman ties are resolved.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
