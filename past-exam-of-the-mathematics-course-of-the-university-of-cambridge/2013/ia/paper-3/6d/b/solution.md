<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the matrix as $M(a,b,x)$. Direct multiplication and inversion give

$$
M(a,b,x)M(a',b',x')=M(a+a',b+b',x+x'+ab'),\qquad
M(a,b,x)^{-1}=M(-a,-b,ab-x).
$$

The identity is $M(0,0,0)$ and all determinants are one, so these formulas verify the [subgroup](../../../../../../subgroup.md) criterion inside $\mathrm{GL}_3(\mathbb R)$. This is the [real Heisenberg group](../../../../../../heisenberg-group.md).

The map $M(a,b,x)\mapsto a$ is a surjective [group homomorphism](../../../../../../group-homomorphism.md) to the additive [group](../../../../../../group-split.md) of real numbers; its kernel is exactly $H$. Hence $H$ is normal and the [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) gives

$$
\boxed{G/H\cong(\mathbb R,+).}
$$

Two matrices commute exactly when $ab'=a'b$. Requiring that relation for every $a',b'$ forces $a=b=0$, while $x$ is unrestricted. Therefore

$$
\boxed{Z(G)=\{M(0,0,x):x\in\mathbb R\}.}
$$

Finally $M(a,b,x)\mapsto(a,b)$ is a surjective [group homomorphism](../../../../../../group-homomorphism.md) to the additive [group](../../../../../../group-split.md) $\mathbb R^2$ with precisely this [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md), giving **$G/Z(G)\cong(\mathbb R^2,+)$**. The central coordinate records noncommutativity: the [group commutator](../../../../../../group-commutator.md) is $M(0,0,ab'-a'b)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
