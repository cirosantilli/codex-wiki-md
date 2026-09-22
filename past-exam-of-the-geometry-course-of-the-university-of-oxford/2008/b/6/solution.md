<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [inflection point](../../../../inflection-point.md) is a smooth point where the tangent line has [intersection multiplicity](../../../../intersection-multiplicity.md) at least three with the curve. For a nonsingular plane curve of degree $n\geq3$, these are the intersections with its [Hessian curve](../../../../hessian-curve-of-a-plane-curve.md), whose degree is $3(n-2)$. The original curve is not a component of its Hessian: otherwise in each graph chart the tangent direction would have zero derivative identically, making the curve locally a line and hence a line globally. Bézout therefore gives the upper bound **$3n(n-2)$**, counting multiplicity. A nonsingular [conic](../../../../conic-section.md) has no inflection points; lines are excluded from this finite-contact definition.

Take $F=y^2z-x^3+xz^2$. Its Hessian determinant is

$$
\det D^2F=8(3xy^2-3x^2z-z^3).
$$

At infinity the curve has only $O=[0:1:0]$, which is an [inflection point](../../../../inflection-point.md): its tangent is $z=0$ and the restricted equation is $-x^3=0$. In the chart $z=1$, substitute $y^2=x^3-x$ into the Hessian equation to obtain

$$
3x^4-6x^2-1=0,\qquad x^2=1\pm\frac2{\sqrt3}.
$$

Thus the full answer is

$$
\boxed{O=[0:1:0],\qquad [x:y:1]\text{ with }x^2=1\pm2/\sqrt3,\quad y=\pm\sqrt{x^3-x}.}
$$

The four complex values of $x$ are distinct and none is $0,1,-1$, so each gives two distinct nonzero values of $y$. Together with $O$ these are all nine inflection points, exhausting the Bézout bound.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
