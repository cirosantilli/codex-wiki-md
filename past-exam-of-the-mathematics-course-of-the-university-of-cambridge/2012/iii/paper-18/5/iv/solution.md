<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The printed construction is not well defined: the next tangent must pass through $x_1$, rather than $x_0$. If $x_0\ne x_1$ and $\ell_1\ne\ell_0$, a second line through $x_0$ cannot also pass through $x_1$, because the unique line through both points is $\ell_0$. Here is a concrete counterexample satisfying all the conic hypotheses. In the affine chart take

$$
C_1:x^2+y^2=1,\qquad C_2:x^2/4+y^2/9=1,
$$

with $\ell_0:x=1$, $x_0=(1,3\sqrt3/2)$ and $x_1=(1,-3\sqrt3/2)$. The second tangent through $x_0$ is $-23x+12\sqrt3y=31$. It does not contain $x_1$: its left side there is $-77$. The conics meet transversely at the four complex points with $x^2=32/5$, $y^2=-27/5$. Thus this is a defect in the original PDF, not just in its conversion.

For the corrected construction, let $\iota_\ell$ exchange the two points of $C_2$ on a fixed tangent line, and let $\iota_x$ exchange the two tangents to $C_1$ through a fixed point of $C_2$. Both projections from $E$ are degree-two morphisms to a [smooth plane conic](../../../../../../smooth-plane-conic.md): for the line projection this follows from intersecting a line with $C_2$, which has no line component. Since $E$ is smooth and the ground field has characteristic zero, their quadratic function-field extensions define regular involutions on the whole curve. At a ramification point “the second” point is the same point, counted with multiplicity. Each switch is an [involution of a degree-two map from a genus one curve](../../../../../../involution-of-a-degree-two-map-from-a-genus-one-curve.md). Hence the corrected step is the everywhere-defined automorphism $F=\iota_x\circ\iota_\ell$.

Choose an origin $O$ on the [genus one curve](../../../../../../genus-one-curve.md). The [Abel-Jacobi map of a genus-one curve](../../../../../../abel-jacobi-map-of-a-genus-one-curve.md) identifies $E$ with $\operatorname{Pic}^0(E)$ by $p\mapsto\mathcal O_E(p-O)$. Fibers of each degree-two projection are linearly equivalent [Weil divisors](../../../../../../weil-divisor.md), since they are pullbacks of points of $\mathbb P^1$. Thus their group sums are constant: for suitable $a,b\in E$,

$$
\iota_\ell(p)=a-p,\qquad \iota_x(p)=b-p,\qquad F(p)=p+(b-a).
$$

This also holds at the ramification points, where $2p=a$ or $2p=b$. Therefore the corrected step is a [translation on an elliptic curve](../../../../../../translation-on-an-elliptic-curve.md). If $F^n(p_0)=p_0$ for one point, then $n(b-a)=0$. It follows that $F^n(p)=p$ for every $p\in E$. **The corrected construction has the [Poncelet porism](../../../../../../poncelet-porism.md): one periodic orbit implies all orbits are periodic, with the same least period.** The literal printed construction fails before this conclusion; the proof establishes the intended, explicitly corrected assertion.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
