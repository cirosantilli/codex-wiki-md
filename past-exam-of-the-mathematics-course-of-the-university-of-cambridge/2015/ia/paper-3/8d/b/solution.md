<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [Heisenberg group](../../../../../../heisenberg-group.md) element as $M(x,y,z)$. Matrix multiplication and inversion give

$$
M(x,y,z)M(x',y',z')=M(x+x',\ y+y'+xz',\ z+z'),\qquad
M(x,y,z)^{-1}=M(-x,-y+xz,-z).
$$

All matrices have [determinant](../../../../../../determinant.md) one. They contain $M(0,0,0)=I$, are closed under multiplication and inverses, and inherit associativity from [matrix multiplication](../../../../../../matrix-multiplication.md); hence they form a [subgroup](../../../../../../subgroup.md) of $GL_3(\mathbb R)$.

Two such matrices commute precisely when $xz'=x'z$. Requiring this for every $x',z'$ forces $x=z=0$. Consequently

$$
\boxed{Z(H)=\{M(0,y,0):y\in\mathbb R\}.}
$$

The map $\pi(M(x,y,z))=(x,z)$ is a surjective [group homomorphism](../../../../../../group-homomorphism.md) to the additive [group](../../../../../../group-split.md) $\mathbb R^2$, with [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) $Z(H)$. Equivalently, it gives the explicit [quotient group](../../../../../../quotient-group.md) isomorphism

$$
\boxed{H/Z(H)\longrightarrow(\mathbb R^2,+),\qquad M(x,y,z)Z(H)\longmapsto(x,z).}
$$

It is well-defined because multiplying by a central element changes only $y$. It is injective because equal $(x,z)$ imply that the quotient of the two matrices is central, and surjectivity follows by taking $y=0$. This also proves the needed instance of the [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) directly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
