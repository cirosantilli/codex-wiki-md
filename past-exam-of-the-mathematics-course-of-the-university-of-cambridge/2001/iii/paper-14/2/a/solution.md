<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $F$ define the [nonsingular plane cubic](../../../../../../nonsingular-plane-cubic.md) and let $H_F=\det\operatorname{Hess}F$ be its [Hessian curve of a plane cubic](../../../../../../hessian-curve-of-a-plane-cubic.md) equation. The [Hessian criterion for a flex](../../../../../../hessian-criterion-for-a-flex.md) applies in the allowed [field characteristic](../../../../../../characteristic-of-a-field.md). Here is the local calculation, so no characteristic-zero argument is needed.

Move any point $P$ to $[0:1:0]$ and its [tangent line](../../../../../../tangent-line.md) to $Z=0$. Smoothness gives a nonzero coefficient $g$ of $Y^2Z$, while the coefficients of $Y^3$ and $XY^2$ vanish. Thus

$$
F(X,Y,0)=aX^3+bX^2Y,\qquad
\operatorname{Hess}F(P)=
\begin{pmatrix}2b&0&f\\0&0&2g\\f&2g&2i\end{pmatrix},
\qquad H_F(P)=-8bg^2.
$$

The [intersection multiplicity](../../../../../../intersection-multiplicity.md) with the [tangent line](../../../../../../tangent-line.md) is at least three precisely when $b=0$, which is precisely $H_F(P)=0$ because the [field characteristic](../../../../../../characteristic-of-a-field.md) is not two. The tangent cannot be a component of a [nonsingular plane cubic](../../../../../../nonsingular-plane-cubic.md).

If $H_F$ vanishes identically, every point is a [flex](../../../../../../inflection-point-of-an-algebraic-plane-curve.md) by this calculation. Otherwise it is a degree-three [homogeneous polynomial](../../../../../../homogeneous-polynomial.md). Its zero locus meets the cubic by [Bézout's theorem](../../../../../../bezout-s-theorem.md); if they share a component, that also supplies a point of intersection. Every such point is smooth and satisfies the criterion, so a [flex](../../../../../../inflection-point-of-an-algebraic-plane-curve.md) exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
