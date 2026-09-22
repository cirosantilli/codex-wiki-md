<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A smooth rank-$r$ [smooth distribution](../../../../../../distribution-differential-geometry.md) $D\subset TM$ is [involutive distribution](../../../../../../involutive-distribution.md) if the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) of two local sections remains a section. It is an [integrable distribution](../../../../../../integrable-distribution.md) if every point lies on an immersed $r$-dimensional [integral manifold](../../../../../../integral-manifold.md) with tangent spaces equal to $D$. The [Frobenius theorem](../../../../../../frobenius-theorem.md) says these conditions are equivalent, and gives local coordinates with $D=\operatorname{span}(\partial_1,\ldots,\partial_r)$.

For necessity, fields tangent to an [integral manifold](../../../../../../integral-manifold.md) have brackets tangent to it: they annihilate functions vanishing on the manifold, and so does their commutator. For sufficiency, induct on $r$. The rank-zero case is immediate. Straighten a nonvanishing local section using the [flow-box theorem](../../../../../../straightening-theorem.md) to obtain $\partial_1\in D$. Choose a frame $\partial_1,Y_2,\ldots,Y_r$ with the $Y_i$ having no $\partial_1$ component. Involutivity gives $\partial_1Y=A Y$ for the column of these fields and a smooth matrix $A$. Solve the matrix ordinary differential equation $\partial_1B=-BA$, with $B=I$ on $x_1=0$. It stays invertible, and $Z=BY$ satisfies $\partial_1Z=0$. On the transverse slice, the $Z_i$ span an involutive rank-$(r-1)$ distribution. The induction hypothesis supplies adapted slice coordinates; extend them independently of $x_1$. These give the required rank-$r$ coordinate distribution and its integral manifolds.

For the [real Heisenberg group](../../../../../../heisenberg-group.md), multiplication is

$$
(x,y,z)(a,b,c)=(x+a,y+b,z+c+xb).
$$

Differentiating left translation at the identity gives its [left-invariant frame of the real Heisenberg group](../../../../../../left-invariant-frame-of-the-real-heisenberg-group.md):

$$
\boxed{E_1=\partial_x,\qquad E_2=\partial_y+x\partial_z,\qquad E_3=\partial_z.}
$$

Then $[E_1,E_2]=E_3$ and the other basis brackets vanish. Since $E_3\notin\operatorname{span}(E_1,E_2)$, the [Heisenberg horizontal distribution](../../../../../../heisenberg-horizontal-distribution.md) is not involutive, hence not integrable by the [Frobenius theorem](../../../../../../frobenius-theorem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
