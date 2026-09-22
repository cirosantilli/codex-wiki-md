<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

The [conjugate group elements](../../../../../conjugate-group-elements.md) relation is $x\sim y$ when $y=gxg^{-1}$ for some $g\in G$. It is reflexive by taking the identity, symmetric because $x=g^{-1}yg$, and transitive because $y=gxg^{-1}$ and $z=hyh^{-1}$ imply $z=(hg)x(hg)^{-1}$. Hence it is an [equivalence relation](../../../../../equivalence-relation.md).

For a finite [group](../../../../../group-split.md), the [centralizer](../../../../../centralizer.md) $C_G(x)=\{g:gx=xg\}$ is a subgroup. The map $g\mapsto gxg^{-1}$ has equal values at $g,h$ exactly when $h^{-1}g\in C_G(x)$. Its fibers are therefore the left cosets of $C_G(x)$, giving

$$
\boxed{|\operatorname{Cl}(x)|=[G:C_G(x)]=\frac{|G|}{|C_G(x)|}}.
$$

By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), this index divides $|G|$. This is also the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) for the conjugation action, with the centralizer as stabilizer.

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
