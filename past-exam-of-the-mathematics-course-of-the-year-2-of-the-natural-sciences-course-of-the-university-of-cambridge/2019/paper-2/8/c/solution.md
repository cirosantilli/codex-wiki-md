<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [cyclic subgroup](../../../../../cyclic-subgroup.md) $A=\langle a\rangle$ has order four and index two. Every index-two [subgroup](../../../../../subgroup.md) is normal: its complement is both the only nontrivial left [coset](../../../../../coset.md) and the only nontrivial right [coset](../../../../../coset.md). Thus [conjugation](../../../../../conjugation.md) by $b$ is an [automorphism](../../../../../automorphism.md) of $A$. It must send its generator $a$ to another element of order four, namely $a$ or $a^3$. Since $b^{-1}=b$,

$$
bab=a\quad\text{or}\quad bab=a^3,
$$

equivalently $ab=ba$ or $ab=ba^3$, as required. Also $b\notin A$, since otherwise $a,b$ could generate at most four elements.

In the commuting case, every word reduces uniquely to $a^jb^\varepsilon$ with $0\leq j<4$ and $\varepsilon\in\{0,1\}$. The eight expressions are distinct because $A$ and $Ab$ are disjoint. Multiplication is addition of the two exponents modulo four and two, respectively. Therefore

$$
\boxed{G\cong C_4\times C_2}.
$$

This gives the [multiplication table](../../../../../multiplication-table.md) independently of any other properties of $G$, proving uniqueness up to [group isomorphism](../../../../../group-isomorphism.md).

In the inversion case, the relation $ba=a^{-1}b$ gives the same eight unique normal forms, now with multiplication

$$
(a^ib^\varepsilon)(a^jb^\eta)
=a^{i+(-1)^\varepsilon j}b^{\varepsilon+\eta},
$$

with exponents reduced modulo four and two. Thus this case also has a uniquely determined [group](../../../../../group-split.md) structure. A faithful geometric realization is the [dihedral group](../../../../../dihedral-group.md) of a square, with $a$ a quarter-turn and $b$ a reflection in a line through opposite edge midpoints. For example, on the plane,

$$
a=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
b=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

These preserve the square with vertices $(\pm1,\pm1)$ and satisfy $a^4=b^2=I$, $bab=a^{-1}$. They generate eight distinct transformations, so

$$
\boxed{G\cong D_4\quad\text{(the symmetry group of a square, of order eight)}}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
