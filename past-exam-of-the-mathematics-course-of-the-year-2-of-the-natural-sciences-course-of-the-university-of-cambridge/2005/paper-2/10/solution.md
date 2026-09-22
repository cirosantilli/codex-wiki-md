<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

A [group representation](../../../../group-representation.md) is a homomorphism $D:G\to\mathrm{GL}(V)$. It is a [reducible representation](../../../../reducible-representation.md) if there is a nonzero proper [invariant subspace](../../../../invariant-subspace.md) of $V$ preserved by every $D(g)$, and an [irreducible representation](../../../../irreducible-representation.md) otherwise. With $S$ invertible,

$$
\widetilde D(gh)=SD(g)D(h)S^{-1}=(SD(g)S^{-1})(SD(h)S^{-1}),
$$

so changing basis gives another representation. Its [character of a representation](../../../../character-of-a-representation.md) is $\chi(g)=\operatorname{tr}D(g)$, and cyclicity of the [trace](../../../../matrix-trace.md) gives $\widetilde\chi(g)=\operatorname{tr}(SD(g)S^{-1})=\chi(g)$.

A [conjugacy class](../../../../conjugacy-class.md) consists of $hgh^{-1}$ as $h$ varies. Since $(hgh^{-1})^k=hg^kh^{-1}$, a power equals the identity exactly when $g^k$ does. Thus [conjugation preserves element order](../../../../conjugation-preserves-element-order.md), including infinite order.

For the square, let $r$ be rotation by $\pi/2$ and $s$ reflection in a horizontal symmetry axis. The [dihedral group](../../../../dihedral-group.md) has the eight elements

$$
e,r,r^2,r^3,s,rs,r^2s,r^3s,\qquad r^4=s^2=e,\quad srs=r^{-1}.
$$

The [conjugacy classes of a finite dihedral group](../../../../conjugacy-classes-of-a-finite-dihedral-group.md) specialize to

$$
\boxed{\{e\},\quad\{r^2\},\quad\{r,r^3\},\quad\{s,r^2s\},\quad\{rs,r^3s\}.}
$$

The two central rotations are singletons. Reflection conjugation reverses rotations, while conjugation by $r$ shifts a reflection exponent by two, giving the two reflection classes.

For finite groups over $\mathbb C$, [character orthogonality](../../../../character-orthogonality.md) and completeness make the [irreducible characters](../../../../irreducible-character.md) a basis of the [class functions](../../../../class-function.md). The latter space has one independent value per conjugacy class. Hence **the square group has five inequivalent irreducible complex representations**. The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) is eight, forcing four one-dimensional representations and one two-dimensional representation. The four scalar choices $r\mapsto\pm1$, $s\mapsto\pm1$ supply the former; the ordinary action on the plane supplies the latter.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
