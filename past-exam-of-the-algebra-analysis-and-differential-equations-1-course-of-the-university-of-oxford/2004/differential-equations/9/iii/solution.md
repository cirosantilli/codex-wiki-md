<h1 id="differential-equations/9/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This is the **[wave equation](../../../../../wave-equation-split.md)**, again taking $y$ as time. Zero is **not unique**: for $k=\pi/2$,

$$
\boxed{u(x,y)=\sin(kx)\sin(ky)}
$$

satisfies $u_{xx}=u_{yy}$ and all the stated [boundary conditions](../../../../../boundary-condition.md). The [initial displacement](../../../../../initial-displacement.md) is zero but the [initial velocity](../../../../../initial-velocity.md) is not prescribed.

A sufficient extra condition is **$u_y(x,0)=0$**. For the resulting homogeneous data use wave energy

$$
E(y)=\frac12\int_0^1(u_y^2+u_x^2)\,dx.
$$

The equation and [integration by parts](../../../../../integration-by-parts.md) give $E'(y)=[u_xu_y]_0^1=0$. At $x=1$ the factor $u_x$ vanishes, and at $x=0$ the factor $u_y$ vanishes because $u(0,y)=0$. The [initial displacement](../../../../../initial-displacement.md) implies $u_x(x,0)=0$, so the extra [initial velocity](../../../../../initial-velocity.md) condition gives $E(0)=0$. Consequently $u_x=u_y=0$ and $u=0$. With the stated boundary regularity, integrate the local [energy conservation](../../../../../conservation-of-energy.md) law over inset rectangles and let their edges approach the boundary; the energy and flux terms converge by [continuity](../../../../../continuous-function.md) of the first derivatives.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
