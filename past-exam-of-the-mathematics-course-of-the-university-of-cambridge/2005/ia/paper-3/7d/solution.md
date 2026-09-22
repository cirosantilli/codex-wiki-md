<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The identity belongs to the [center of a group](../../../../../center-of-a-group.md). If $a,b$ are central, then for every $g\in G$,

$$
g(ab^{-1})=a\,gb^{-1}=ab^{-1}g,
$$

so the center is a [subgroup](../../../../../subgroup.md). For a central $a$, $gag^{-1}=a$ for every $g$, giving $gZ(G)g^{-1}=Z(G)$. Thus **the center is a [normal subgroup](../../../../../normal-subgroup.md)**.

Write a [matrix](../../../../../matrix.md) of the [Heisenberg group](../../../../../heisenberg-group.md) as $h(x,y,z)$. Direct [matrix multiplication](../../../../../matrix-multiplication.md) and inversion give

$$
h(x,y,z)h(a,b,c)=h(x+a,y+b+xc,z+c),
\qquad
h(x,y,z)^{-1}=h(-x,xz-y,-z).
$$

The identity is $h(0,0,0)$ and each [matrix](../../../../../matrix.md) has [determinant](../../../../../determinant.md) one, so these formulas show closure under products and inverses inside $GL_3(\mathbb R)$. Hence $H$ is a [subgroup](../../../../../subgroup.md).

The two products $h(x,y,z)h(a,b,c)$ and $h(a,b,c)h(x,y,z)$ differ only in their upper-right entries, by $xc-az$. Commutation with every $h(a,b,c)$ therefore requires $xc=az$ for all real $a,c$. Setting $a=0,c=1$ forces $x=0$; setting $a=1,c=0$ forces $z=0$. These conditions are also sufficient. Thus

$$
\boxed{Z(H)=\{h(0,y,0):y\in\mathbb R\}.}
$$

Define the surjective [group homomorphism](../../../../../group-homomorphism.md) $F:H\to(\mathbb R^2,+)$ by $F(h(x,y,z))=(x,z)$. The multiplication formula gives $F(hh')=F(h)+F(h')$, and its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is precisely $Z(H)$. The [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) yields

$$
\boxed{H/Z(H)\cong(\mathbb R^2,+),\qquad
h(x,y,z)Z(H)\longmapsto(x,z).}
$$

This [center quotient of the real Heisenberg group](../../../../../center-quotient-of-the-real-heisenberg-group.md) can also be checked directly: two elements have the same $(x,z)$ coordinates exactly when they differ by multiplication by a central element, and quotient multiplication adds these coordinates.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
