<h1 id="20/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [angles](../../../../../../angle.md) in the PDF are measured from the vertical normal to the interface. The horizontal displacements of the two path segments are $d_1\tan\theta$ and $d_2\tan\phi$, while their [lengths](../../../../../../length.md) are $d_1\sec\theta$ and $d_2\sec\phi$. Thus the geometric constraint and travel [time](../../../../../../time-in-physics.md) are

$$
g(\theta,\phi)=d_1\tan\theta+d_2\tan\phi=D,\qquad T(\theta,\phi)=\frac{2d_1\sec\theta+\sqrt2d_2\sec\phi}{c}.
$$

The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations $\nabla T=\lambda\nabla g$ give

$$
\frac{2d_1}{c}\sec\theta\tan\theta=\lambda d_1\sec^2\theta,\qquad\frac{\sqrt2d_2}{c}\sec\phi\tan\phi=\lambda d_2\sec^2\phi.
$$

Cancelling the positive geometric factors gives $\lambda=2\sin\theta/c=\sqrt2\sin\phi/c$, hence

$$
\boxed{\sin\phi=\sqrt2\sin\theta.}
$$

This is [Snell's law](../../../../../../snell-s-law.md), $\sin\theta/(c/2)=\sin\phi/(c/\sqrt2)$. The relation depends only on the ratio of the two [speeds](../../../../../../speed.md), so changing $D,d_1,d_2$ leaves the relation unchanged; it changes which [angles](../../../../../../angle.md) satisfy it together with the geometric constraint.

For a minimum check, let $u$ be the horizontal distance to the crossing [point](../../../../../../point-geometry.md). Then

$$
T(u)=\frac2c\sqrt{u^2+d_1^2}+\frac{\sqrt2}{c}\sqrt{(D-u)^2+d_2^2},
$$

and

$$
T''(u)=\frac{2d_1^2}{c(u^2+d_1^2)^{3/2}}+\frac{\sqrt2d_2^2}{c((D-u)^2+d_2^2)^{3/2}}>0.
$$

Thus the travel [time](../../../../../../time-in-physics.md) is a [strictly convex function](../../../../../../strictly-convex-function.md) of $u$, and its [stationary point](../../../../../../stationary-point.md) is the unique global minimum. For positive $D,d_1,d_2$, $T'(0)<0<T'(D)$, placing the crossing between the two endpoint projections.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [20](../../../20.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
