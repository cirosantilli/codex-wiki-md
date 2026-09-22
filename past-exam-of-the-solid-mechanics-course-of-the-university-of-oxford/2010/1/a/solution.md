<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [homogeneous hyperelastic material](../../../../homogeneous-hyperelastic-material.md) has a stored energy per reference [volume](../../../../volume.md) $W(F)$ depending on the local [deformation gradient](../../../../deformation-gradient.md) but not explicitly on the material point. Its first Piola-Kirchhoff response is

$$
\boxed{\widehat T(F)=DW(F),\qquad T_{i\alpha}=\partial W/\partial F_{i\alpha}.}
$$

A superposed rigid rotation changes the observer's description without changing the energy of the [deformation](../../../../deformation-mechanics.md). [Material frame indifference](../../../../material-frame-indifference.md) is therefore

$$
\boxed{W(QF)=W(F)\quad(F\in\mathbb M_+^{3\times3},\ Q\in\mathrm{SO}(3)).}
$$

This left-rotation invariance is distinct from a [material isotropy](../../../../material-isotropy.md) assumption on right rotations. Differentiate it in an arbitrary matrix direction $H$:

$$
DW(QF):(QH)=DW(F):H.
$$

The [Frobenius inner product](../../../../frobenius-inner-product.md) then gives $Q^T\widehat T(QF)=\widehat T(F)$, proving $\widehat T(QF)=Q\widehat T(F)$.

For the converse, that stress covariance makes the [derivative](../../../../derivative.md) in $F$ of $W(QF)-W(F)$ zero. The positive-[determinant](../../../../determinant.md) matrices form a [connected set](../../../../connected-set.md), as also follows from [polar decomposition](../../../../polar-decomposition.md), so this difference is a constant $c(Q)$ independent of $F$. Composition gives $c(Q_1Q_2)=c(Q_1)+c(Q_2)$. For fixed $F$, [continuity](../../../../continuous-function.md) of $W$ and [compactness](../../../../compact-space.md) of $\mathrm{SO}(3)$ make $c$ bounded. But $c(Q^n)=nc(Q)$ for every positive integer, forcing $c(Q)=0$. Thus **stress covariance and frame indifference of the energy are equivalent**. [Compactness](../../../../compact-space.md) removes the possible additive energy constant in the converse.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
