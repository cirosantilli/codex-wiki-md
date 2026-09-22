<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here the star means entrywise [complex conjugation](../../../../complex-conjugation.md), not [Hermitian conjugation](../../../../hermitian-conjugation.md). Put $s=g_3$ and $r=g_1g_3$. Since $\alpha^3=1$ and $1+\alpha+\alpha^2=0$,

$$
r=\begin{pmatrix}\alpha^2&0\\0&\alpha\end{pmatrix},\qquad
s=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
r^3=s^2=I,\qquad srs=r^{-1}.
$$

The generators are $g_1=rs$, $g_2=r^2s$ and $g_3=s$. Moving every occurrence of $s$ to the right using $sr=r^{-1}s$ reduces every word to $r^k$ or $r^ks$ with $k=0,1,2$. The three diagonal [matrices](../../../../matrix.md) are distinct, as are the three off-diagonal [matrices](../../../../matrix.md), so

$$
\boxed{G=\{I,r,r^2,s,rs,r^2s\},\qquad |G|=6.}
$$

For an explicit [group isomorphism](../../../../group-isomorphism.md), send $r$ to $(123)$ and $s$ to $(12)$ in the [symmetric group](../../../../symmetric-group.md) $S_3$, composing [permutations](../../../../permutation.md) from right to left. These [permutations](../../../../permutation.md) satisfy the same relations and generate $S_3$. The normal forms above then give an isomorphism; in particular $g_1\mapsto(13)$, $g_2\mapsto(23)$ and $g_3\mapsto(12)$.

Conjugation by $s$ exchanges $r$ with $r^2$, and conjugation by $r$ cycles the three reflections. The [conjugacy classes](../../../../conjugacy-class.md) are therefore

$$
\boxed{\{I\},\qquad \{r,r^2\},\qquad \{s,rs,r^2s\}=\{g_1,g_2,g_3\}.}
$$

Their sizes are $1,2,3$, respectively. They correspond to the identity, three-cycles and [transpositions](../../../../transposition-permutation.md) in $S_3$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
