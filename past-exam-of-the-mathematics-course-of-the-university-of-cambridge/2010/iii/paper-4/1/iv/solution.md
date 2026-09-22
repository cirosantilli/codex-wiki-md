<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use rightmost-first composition of [permutations](../../../../../../permutation.md), and let

$$
a=(1\,2\,\cdots\,n),\qquad b=(n-1\,n-2\,\cdots\,1).
$$

For $n\ge2$, direct evaluation gives $ab=(1\,n)$. Conjugating this [transposition](../../../../../../transposition-permutation.md) by powers of $a$ yields the [transpositions](../../../../../../transposition-permutation.md) between consecutive letters around the cycle, including $(1\,2),(2\,3),\ldots,(n-1\,n)$.

Put $s_i=(i\,i+1)$. For $i<j$,

$$
(i\,j)=s_i s_{i+1}\cdots s_{j-2}s_{j-1}s_{j-2}\cdots s_{i+1}s_i.
$$

Thus the adjacent [transpositions](../../../../../../transposition-permutation.md) generate every [transposition](../../../../../../transposition-permutation.md), and [permutation cycle](../../../../../../permutation-cycle.md) decomposition shows that [transpositions](../../../../../../transposition-permutation.md) generate the [symmetric group](../../../../../../symmetric-group.md). Therefore $\langle a,b\rangle=S_n$.

For the final lower bound, associate a [graph](../../../../../../graph-split.md) to a family of [transpositions](../../../../../../transposition-permutation.md): its vertices are the letters and its edges are the swapped pairs. Every generator preserves every connected component, so generation of $S_n$ requires that [graph](../../../../../../graph-split.md) to be connected. A connected [graph](../../../../../../graph-split.md) on $n$ vertices needs at least $n-1$ edges: adding an edge can reduce the number of components by at most one, starting from $n$ isolated vertices. The adjacent [transpositions](../../../../../../transposition-permutation.md) supply exactly $n-1$ edges. Equivalently, [transpositions on a connected graph generate the symmetric group](../../../../../../transpositions-on-a-connected-graph-generate-the-symmetric-group.md). Hence

$$
\boxed{\text{The least number of transpositions generating }S_n\text{ is }n-1.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
