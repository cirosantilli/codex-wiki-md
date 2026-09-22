<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [nonsingular point of an algebraic curve](../../../../nonsingular-point-of-an-algebraic-curve.md) $p$ is an [inflection point of an algebraic plane curve](../../../../inflection-point-of-an-algebraic-plane-curve.md), or [flex](../../../../inflection-point-of-an-algebraic-plane-curve.md), if its [projective tangent line](../../../../tangent-line-to-a-projective-plane-curve.md) has contact of order at least three:

$$
I_p(C,T_pC)\geq3.
$$

Here the [projective tangent line](../../../../tangent-line-to-a-projective-plane-curve.md) must not be a component of $C$. Ordinary tangency has contact order two.

Let $C=V(F)$, where $F$ is a [homogeneous polynomial](../../../../homogeneous-polynomial.md) of degree $d\geq2$. Its [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md) is defined by

$$
H_F=\det\begin{pmatrix}
F_{xx}&F_{xy}&F_{xz}\\
F_{yx}&F_{yy}&F_{yz}\\
F_{zx}&F_{zy}&F_{zz}
\end{pmatrix}=0.
$$

Each entry has degree $d-2$, so a nonzero $H_F$ has degree $3(d-2)$. By the [Hessian criterion for a flex](../../../../hessian-criterion-for-a-flex.md), the [flexes](../../../../inflection-point-of-an-algebraic-plane-curve.md) are exactly the points of $C\cap V(H_F)$. The stated no-common-component assumption and [Bézout's theorem](../../../../bezout-s-theorem.md) therefore give

$$
\boxed{\#\{\text{distinct flexes of }C\}\leq3d(d-2).}
$$

This counts distinct points; higher contact can use more than one unit of [intersection multiplicity](../../../../intersection-multiplicity.md) at a single point.

For completeness, the [Hessian criterion for a flex](../../../../hessian-criterion-for-a-flex.md) follows by putting $p=[0:0:1]$ and $T_pC=\{y=0\}$, with $F_y(p)\ne0$. The [Euler theorem for homogeneous functions](../../../../euler-theorem-for-homogeneous-functions.md) gives $F_{xz}(p)=F_{zz}(p)=0$ and $F_{yz}(p)=(d-1)F_y(p)$, whence

$$
H_F(p)=-(d-1)^2F_y(p)^2F_{xx}(p).
$$

The restriction $F(x,0,1)$ already has vanishing constant and linear terms. Its quadratic term vanishes exactly when the [intersection multiplicity](../../../../intersection-multiplicity.md) with the tangent is at least three, proving the criterion.

For $d\geq3$ the bound is the actual [maximum number of flexes of a smooth plane curve](../../../../maximum-number-of-flexes-of-a-smooth-plane-curve.md): a general nonsingular curve has only contact of order three, and the corresponding intersections with its [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md) are simple. One way to see genericity is to vary a point and a line through it, a three-dimensional family. Contact of order at least four imposes four independent linear conditions on the coefficients of a degree-$d$ equation for $d\geq3$. Thus the locus of equations with such contact is a proper exceptional locus. Locally, if the curve is $y=h(x)$, its [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md) restricted to $C$ is a nonvanishing factor times $h''(x)$; contact exactly three gives a simple zero.

A nonsingular [plane conic](../../../../plane-conic.md) has no [flexes](../../../../inflection-point-of-an-algebraic-plane-curve.md), agreeing with the formula at $d=2$. A line is excluded from this formulation: its tangent is itself and its [Hessian matrix](../../../../hessian-matrix.md) is zero, so the no-common-component hypothesis fails. The formula is therefore intended for $d\geq2$, rather than giving the meaningless negative value at $d=1$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
