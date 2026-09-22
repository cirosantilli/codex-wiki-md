<h1 id="9/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Label the triangle vertices $1,2,3$ counterclockwise. Let $R$ rotate by $2\pi/3$ counterclockwise and let $m$ reflect across the line through vertex 1 and the midpoint of the opposite side. The [dihedral group](../../../../../dihedral-group.md) has elements $I,R,R^2,m,Rm,R^2m$, with $R^3=m^2=I$ and $mRm=R^{-1}$.

The action on vertices identifies them with these [permutations](../../../../../permutation.md), with the rightmost operation applied first:

$$
\boxed{\begin{array}{c|c|l}
\text{element}&\text{permutation}&\text{geometric action}\\\hline
I&e&\text{identity}\\
R&(123)&\text{rotation through }120^\circ\\
R^2&(132)&\text{rotation through }240^\circ\\
m&(23)&\text{reflection fixing vertex 1}\\
Rm&(12)&\text{reflection fixing vertex 3}\\
R^2m&(13)&\text{reflection fixing vertex 2}
\end{array}.}
$$

The minimal number of generators is two, and $\{R,m\}$ is one minimal generating set. They produce every displayed element. A one-element generating set would make the group cyclic, but every nonidentity element has order two or three, never six.

The vertex-action map preserves composition, hence is a [group homomorphism](../../../../../group-homomorphism.md) from $D_3$ to the [symmetric group](../../../../../symmetric-group.md) $S_3=\Sigma_3$. The displayed actions are all six distinct permutations of three vertices, so the map is both injective and surjective. Therefore

$$
\boxed{D_3\cong S_3.}
$$

This identification uses the convention $|D_3|=6$, with the subscript counting polygon vertices.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
