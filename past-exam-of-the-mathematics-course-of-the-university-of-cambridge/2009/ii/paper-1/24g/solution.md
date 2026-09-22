<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

A [rational map](../../../../../rational-map-complex-analysis.md) $V\dashrightarrow\mathbb P^m$ is a morphism on a nonempty open subset of $V$, with two descriptions identified if they agree on a dense open subset. It can be represented there by rational homogeneous coordinate functions not all zero. A point is regular for the map if it extends as a [morphism](../../../../../morphism.md) on an open neighbourhood of that point.

For the given [projective Cremona transformation](../../../../../projective-cremona-transformation.md), the three products vanish simultaneously exactly at the three coordinate vertices. Away from them they define a [regular map](../../../../../morphism-of-algebraic-varieties.md). At $(1:0:0)$ consider $[1:t:st]$ as $t\to0$, with $s\ne0$. Its image tends to $[0:s:1]$, which depends on $s$. No regular extension could have these different limiting values. Algebraically these curves lie in its domain for $t\ne0$ and a regular extension must give the same specialization at their common vertex, so the obstruction also works over any infinite characteristic-zero field. The other vertices follow by cyclic symmetry. On the torus $X_0X_1X_2\ne0$, applying the map twice gives

$$
[X_0^2X_1X_2:X_0X_1^2X_2:X_0X_1X_2^2]=[X_0:X_1:X_2].
$$

It is therefore a [birational map](../../../../../birational-map.md) and is its own rational inverse.

Use coordinates $[A:B:C]$ on the target. Substitution in the quintic gives

$$
F(BC,AC,AB)=A^2B^2C^2\,Q(A,B,C),\qquad Q=AC^3+A^3B+B^3C.
$$

Thus on the torus its image is the plane quartic $Q=0$. This quartic is nonsingular even over the algebraic closure. Its partial derivatives are $C^3+3A^2B$, $A^3+3B^2C$ and $3AC^2+B^3$. If one coordinate vanishes at a common zero of these partials, all vanish. If none vanishes, multiplying the three equations gives $A^3B^3C^3=-27A^3B^3C^3$, impossible in characteristic zero. Hence there is no projective singular point.

A smooth plane curve is geometrically irreducible: if it had two positive-degree components, [Bézout theorem](../../../../../bezout-s-theorem.md) over the algebraic closure would give an intersection point, and the product equation has zero gradient there; a repeated factor also makes the gradient vanish along its component. Therefore this quartic is irreducible. Its torus part is dense and is identified by the [projective Cremona transformation](../../../../../projective-cremona-transformation.md) with the torus part of $V$. No coordinate line is a component of $V$, since restricting $F$ to each coordinate line leaves a nonzero monomial. Consequently every component meets the torus, and its torus part is already irreducible. **$V$ is irreducible and birational to the nonsingular quartic $AC^3+A^3B+B^3C=0$.**

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
