<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

The [Klein four-group](../../../../klein-four-group.md) has multiplication table

$$
\begin{array}{c|cccc}
 &1&a&b&c\\\hline
1&1&a&b&c\\
a&a&1&c&b\\
b&b&c&1&a\\
c&c&b&a&1
\end{array}.
$$

Since it is abelian, every [conjugacy class](../../../../conjugacy-class.md) is a singleton: $\{1\},\{a\},\{b\},\{c\}$. An [irreducible representation](../../../../irreducible-representation.md) is a nonzero representation whose only invariant subspaces are zero and the whole representation space. For a [finite group](../../../../finite-group.md), the number of inequivalent complex irreducible representations equals the number of conjugacy classes, so there are four here.

A one-dimensional representation sends the involutions $a,b$ to signs, independently. All four choices are

$$
\chi_{pq}(1)=1,\quad\chi_{pq}(a)=(-1)^p,\quad\chi_{pq}(b)=(-1)^q,\quad\chi_{pq}(c)=(-1)^{p+q},\qquad p,q\in\{0,1\}.
$$

They are distinct irreducible representations, exhausting the four possibilities. The [character table of the Klein four-group](../../../../character-table-of-the-klein-four-group.md) is

$$
\boxed{\begin{array}{c|rrrr}
 &1&a&b&c\\\hline
\chi_{00}&1&1&1&1\\
\chi_{01}&1&1&-1&-1\\
\chi_{10}&1&-1&1&-1\\
\chi_{11}&1&-1&-1&1
\end{array}.}
$$

The specified diagonal [matrices](../../../../matrix.md) obey $D(a)^2=D(b)^2=I$, commute, and satisfy $D(a)D(b)=D(c)$, so the group relations prove that $D$ is a [group representation](../../../../group-representation.md). Its coordinate axes are invariant lines carrying respectively $\chi_{01},\chi_{10},\chi_{11}$. Therefore

$$
\boxed{D\cong\chi_{01}\oplus\chi_{10}\oplus\chi_{11}.}
$$

The [trivial representation](../../../../trivial-representation.md) $\chi_{00}$ is absent. If $H$ denotes the four-row character [matrix](../../../../matrix.md) above, direct row products give $HH^T=4I$. This verifies [character orthogonality](../../../../character-orthogonality.md):

$$
\frac14\sum_{g\in V}\overline{\chi_{pq}(g)}\chi_{rs}(g)=\delta_{pr}\delta_{qs}.
$$

The character of $D$ is $(3,-1,-1,-1)$, whose inner products with the four rows are $0,1,1,1$, independently confirming the decomposition. All these irreducibles are real as well: commuting real involutions can be simultaneously diagonalized into their real sign eigenspaces.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
