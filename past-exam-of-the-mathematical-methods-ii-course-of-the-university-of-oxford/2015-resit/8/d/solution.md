<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $C$ to be a simple closed, piecewise smooth curve oriented counterclockwise around its interior $D$. [Green's theorem](../../../../green-theorem.md) applied to $P=-y$ and $Q=x$ gives

$$
\oint_C(x\,dy-y\,dx)=\iint_D\left(\frac{\partial x}{\partial x}-\frac{\partial(-y)}{\partial y}\right)dx\,dy=2\iint_Ddx\,dy=2\mathcal A.
$$

The orientation is essential: a clockwise unit circle gives $-2\pi$, whereas twice its ordinary unsigned area is $+2\pi$. For a nonsimple curve, the corresponding formula concerns signed area with winding multiplicity rather than one unsigned enclosed area.

For positive semiaxes $a,b$, parametrize the [ellipse](../../../../ellipse.md) counterclockwise by $x=a\cos\theta$, $y=b\sin\theta$, $0\le\theta\le2\pi$. Then

$$
x\,dy-y\,dx=ab\cos^2\theta\,d\theta+ab\sin^2\theta\,d\theta=ab\,d\theta.
$$

Hence $2\mathcal A=\int_0^{2\pi}ab\,d\theta=2\pi ab$, and

$$
\boxed{\mathcal A=\pi ab}.
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
