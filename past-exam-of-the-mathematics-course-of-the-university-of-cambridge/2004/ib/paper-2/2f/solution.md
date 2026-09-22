<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

We prove [Simplicity of the alternating group A5](../../../../../simplicity-of-the-alternating-group-a5.md) by finding all its [conjugacy classes](../../../../../conjugacy-class.md). The [alternating group](../../../../../alternating-group.md) has [group order](../../../../../order-of-a-finite-group.md) $|A_5|=5!/2=60$. Its even [permutations](../../../../../permutation.md) have cycle types $1$, $(abc)$, $(ab)(cd)$ and $(abcde)$. There are $\binom53\cdot2=20$ three-cycles, $5\cdot3=15$ products of disjoint transpositions, and $4!=24$ five-cycles.

For a three-cycle, a commuting [permutation](../../../../../permutation.md) must rotate its three-element support and may interchange the two fixed points. Its [centralizer](../../../../../centralizer.md) in $S_5$ has order six, and only the three rotations are even. Thus its [conjugacy class](../../../../../conjugacy-class.md) in $A_5$ has size $60/3=20$ and contains every three-cycle. The [centralizer](../../../../../centralizer.md) of $(12)(34)$ in $S_5$ has order eight: one may interchange the two pairs and independently interchange the elements within each pair. It contains the odd element $(12)$, so exactly half of these commuting elements are even. The [conjugacy class](../../../../../conjugacy-class.md) in $A_5$ consequently has size $60/4=15$. A [permutation](../../../../../permutation.md) commuting with a five-cycle is determined by the image of one point and must be a power of that cycle. All five powers are even, so each such [conjugacy class](../../../../../conjugacy-class.md) has size $60/5=12$. The 24 five-cycles form exactly two classes.

A [normal subgroup](../../../../../normal-subgroup.md) contains the identity and is a union of whole [conjugacy classes](../../../../../conjugacy-class.md). Its possible orders therefore lie in

$$
1+\{0,12,24\}+\{0,15\}+\{0,20\}
=\{1,13,16,21,25,28,33,36,40,45,48,60\}.
$$

By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), its order must divide 60. Only 1 and 60 in this list do so. Hence **$A_5$ has no proper nontrivial [normal subgroup](../../../../../normal-subgroup.md) and is a [simple group](../../../../../simple-group.md)**.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
