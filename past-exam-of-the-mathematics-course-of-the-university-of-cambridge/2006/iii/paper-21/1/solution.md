<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $L=L_1\cap L_2$, and let $j:L\hookrightarrow M$ be inclusion. The [transverse intersection theorem](../../../../../transverse-intersection-theorem.md) makes $L$ a smooth [submanifold](../../../../../submanifold.md) without boundary, with

$$
T_xL=T_xL_1\cap T_xL_2,\qquad
\operatorname{codim}_{\mathbb R}L
=\operatorname{codim}_{\mathbb R}L_1+\operatorname{codim}_{\mathbb R}L_2.
$$

It is compact because it is a closed subset of either compact input [submanifold](../../../../../submanifold.md).

Write $\nu_r=TM|_{L_r}/TL_r$. On $L$, consider the bundle map

$$
TM|_L\longrightarrow\nu_1|_L\oplus\nu_2|_L,\qquad
v\longmapsto(v\bmod TL_1,\ v\bmod TL_2).
$$

Its kernel is $TL$, and it is onto because $TL_1+TL_2=TM$ at every intersection point. Thus the [normal bundle of a transverse intersection](../../../../../normal-bundle-of-a-transverse-intersection.md) has the actual bundle isomorphism

$$
\nu(j)\cong\nu_1|_L\oplus\nu_2|_L.
$$

Transfer the direct-sum [complex structure](../../../../../complex-structure.md) $J_1\oplus J_2$ through this isomorphism. This supplies a [complex structure](../../../../../complex-structure.md) on the [normal bundle](../../../../../normal-bundle.md) itself, not merely after stabilization.

Geometrically, multiply the two classes by forming their external product in $M\times M$ and pulling it back along the diagonal $\Delta:M\to M\times M$. The transversality hypothesis is precisely what makes the inverse image of $L_1\times L_2$ under $\Delta$ the [submanifold](../../../../../submanifold.md) $L$. The [normal bundle](../../../../../normal-bundle.md) of this inverse image is the direct sum just calculated. Multiplication of the corresponding [Thom classes](../../../../../thom-class.md) agrees with the [Thom class](../../../../../thom-class.md) of this direct sum, so the [complex cobordism product represented by transverse intersections](../../../../../complex-cobordism-product-represented-by-transverse-intersections.md) is

$$
\boxed{[L_1,i_1,\nu_1]*[L_2,i_2,\nu_2]
=[L_1\cap L_2,\ j,\ \nu_1|_L\oplus\nu_2|_L].}
$$

If the inputs have complex normal ranks $a,b$, the product has degree $2(a+b)$. If they are disjoint, the representative is empty and the product is zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
