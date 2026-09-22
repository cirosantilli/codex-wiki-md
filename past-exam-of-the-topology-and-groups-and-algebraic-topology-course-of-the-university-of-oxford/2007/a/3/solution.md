<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

One standard five-operation version of the [Tietze transformations](../../../../tietze-transformations.md) is: invert a relator; conjugate a relator by a word; multiply a relator on either side by another relator; insert or delete the empty relator; and introduce or eliminate a generator together with a defining relation $y=w$, where $w$ uses the other generators and an eliminated generator occurs nowhere else. The elementary relator operations are reversible. Renaming and reordering the generators and relators is harmless. The Tietze theorem states that two finite presentations define isomorphic groups exactly when they are related by a finite sequence of these transformations.

For a [connected](../../../../connected-space.md) cell complex with one vertex, take one generator for each oriented one-cell and one relator from the attaching loop of each two-cell. Higher-dimensional cells do not change the [fundamental group](../../../../fundamental-group.md). This is the cellular presentation theorem, obtained by applying van Kampen to the two-skeleton. Conversely a finite presentation is realized by a bouquet of its generator circles with one disk attached along each relator word, giving a finite [connected](../../../../connected-space.md) complex with the required [fundamental group](../../../../fundamental-group.md).

Triangulate each relator polygon by adding diagonals from one boundary vertex. Each diagonal is a new one-cell, and every triangular two-cell has an attaching word of length at most three. Algebraically, for a word $s_1\cdots s_\ell$ with $\ell\ge4$, introduce successive partial-product generators $y_2,\ldots,y_{\ell-2}$. Use relators

$$
s_1s_2y_2^{-1},\qquad y_{j-1}s_jy_j^{-1}\ (3\le j\le\ell-2),\qquad y_{\ell-2}s_{\ell-1}s_\ell.
$$

Eliminating the new generators recovers the original word; words already of length at most three need no change. This proves the triangular-presentation claim geometrically and algebraically.

For the [free abelian group](../../../../free-abelian-group.md) of rank two, use

$$
\boxed{\langle a,b,c\mid abc^{-1},\ ca^{-1}b^{-1}\rangle}.
$$

Its two relations say $c=ab=ba$. For the requested transformation sequence, replace the second relator by the product of the first and second, freely reducing it to $aba^{-1}b^{-1}$. Invert the first relator, giving $cb^{-1}a^{-1}$, the definition $c=ab$. Eliminate $c$ together with this defining relation. The remaining presentation is exactly the stated two-generator [commutator](../../../../commutator.md) presentation.

The construction is a [triangular group presentation](../../../../triangular-group-presentation.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../split.md)
5. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
