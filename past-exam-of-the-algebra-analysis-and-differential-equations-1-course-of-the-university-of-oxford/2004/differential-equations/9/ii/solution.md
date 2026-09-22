<h1 id="differential-equations/9/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This is **[Laplace's equation](../../../../../laplace-equation.md)**. Zero is **not unique**: with $k=\pi/2$,

$$
\boxed{u(x,y)=\sin(kx)\sinh(ky)}
$$

is nonzero and [harmonic](../../../../../harmonic-function.md). It vanishes on $y=0$ and $x=0$, while $u_x(1,y)=k\cos(k)\sinh(ky)=0$.

A sufficient additional condition is **$u(x,1)=0$** on the top edge. [Green's first identity](../../../../../green-s-first-identity.md) then gives

$$
\int_D|\nabla u|^2\,dx\,dy=\int_{\partial D}u\,\partial_nu\,ds-\int_Du\Delta u\,dx\,dy=0.
$$

On the bottom, left and top edges $u=0$; on the right edge the normal derivative is zero. Thus the [gradient](../../../../../gradient.md) vanishes and $u$ is constant; the bottom value makes that constant zero. For $C^2(D)\cap C^1(\overline D)$, apply the identity on inset rectangles and pass to the boundary using [continuity](../../../../../continuous-function.md) of the function and its [gradient](../../../../../gradient.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [9](../../9.md)
3. [Differential equations](../../../differential-equations.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
