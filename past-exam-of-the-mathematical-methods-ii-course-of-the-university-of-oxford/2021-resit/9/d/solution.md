<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume a simple, piecewise smooth closed [curve](../../../../curve.md) oriented counterclockwise around its enclosed region $D$. Apply [Green's theorem](../../../../green-theorem.md) with $P=-y$ and $Q=x$:

$$
\oint_C(x\,dy-y\,dx)
=\iint_D(Q_x-P_y)\,dx\,dy
=\iint_D2\,dx\,dy
=\boxed{2\,\operatorname{area}(D).}
$$

The orientation assumption is essential. A clockwise unit [circle](../../../../circle.md), $x=\cos\theta$, $y=-\sin\theta$ for $0\le\theta\le2\pi$, gives $-2\pi$ although its enclosed [area](../../../../surface-area.md) is $\pi$. For a self-intersecting [curve](../../../../curve.md) the same [line integral](../../../../line-integral.md) measures twice the [signed area](../../../../signed-area.md), with multiplicity, rather than necessarily twice an ordinary enclosed [area](../../../../surface-area.md).

For positive semiaxes $a,b$, the [ellipse](../../../../ellipse.md) has the counterclockwise [parametrization](../../../../parametric-equation.md) $x=a\cos\theta$, $y=b\sin\theta$. Then

$$
x\,dy-y\,dx
=ab(\cos^2\theta+\sin^2\theta)\,d\theta=ab\,d\theta.
$$

Therefore

$$
\boxed{\operatorname{area}(\text{ellipse})=\frac12\int_0^{2\pi}ab\,d\theta=\pi ab.}
$$

If nonzero signed constants are allowed in place of positive semiaxes, the geometric [area](../../../../surface-area.md) is $\pi|ab|$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [9](../../9.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
