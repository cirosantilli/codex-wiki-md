<h1 id="differential-equations/8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention $A u_{xx}+2B u_{xy}+C u_{yy}=0$, with discriminant $B^2-AC$. Here $A=1$, $B=0$, $C=\operatorname{sign}(y)$.

For $y>0$, the discriminant is $-1<0$, so the equation is an [elliptic partial differential equation](../../../../../elliptic-partial-differential-equation.md), already in the canonical [Laplace equation](../../../../../laplace-equation.md) form $u_{xx}+u_{yy}=0$.

For $y<0$, the discriminant is $1>0$, so it is a [hyperbolic partial differential equation](../../../../../hyperbolic-partial-differential-equation.md), the [wave equation](../../../../../wave-equation-split.md) $u_{xx}-u_{yy}=0$. Introduce characteristic coordinates

$$
\xi=x+y,\qquad\eta=x-y.
$$

Then $\partial_x=\partial_\xi+\partial_\eta$ and $\partial_y=\partial_\xi-\partial_\eta$, giving

$$
u_{xx}-u_{yy}=4u_{\xi\eta}=0.
$$

On $y=0$, the discriminant vanishes and the principal part has rank one; the degenerate [parabolic type](../../../../../parabolic-partial-differential-equation.md) is $u_{xx}=0$. This is an interface line, rather than an open parabolic subdomain. Thus

$$
\boxed{\begin{array}{c|c|c}
y>0&\text{elliptic}&u_{xx}+u_{yy}=0\\
y<0&\text{hyperbolic}&u_{\xi\eta}=0\\
y=0&\text{degenerate parabolic}&u_{xx}=0
\end{array}}
$$

This is a [mixed-type partial differential equation](../../../../../mixed-type-partial-differential-equation.md). The classification concerns the principal part and remains meaningful even though the coefficient jumps at the interface.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
