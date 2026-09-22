<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The homogeneous [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has powers $x^r$ with $r(r-1)+2r-2=(r-1)(r+2)=0$. Boundedness at zero selects $x$, and boundedness at infinity selects $x^{-2}$. Put $G=Ax$ for $x<\zeta$ and $G=Bx^{-2}$ for $x>\zeta$. Continuity gives $B=A\zeta^3$. Since the operator is $L=(x^2\,d/dx)'-2$, the required delta-function normalization is $\zeta^2[G_x]_{\zeta^-}^{\zeta^+}=1$. Thus $-3A\zeta^2=1$, giving the [bounded Green kernel for a radial Euler operator](../../../../bounded-green-kernel-for-a-radial-euler-operator.md):

$$
\boxed{G(x,\zeta)=\begin{cases}-x/(3\zeta^2),&0<x<\zeta,\\-\zeta/(3x^2),&\zeta<x<\infty.\end{cases}}
$$

In the requested notation, $\boxed{a=1,\ b=-2,\ c=1,\ d=-2,\ k_-=k_+=-1/3}$. The two expressions agree at $x=\zeta$.

With ordinary measure $d\zeta$, the solution is

$$
\boxed{y(x)=\int_0^\infty G(x,\zeta)f(\zeta)d\zeta=-\frac1{3x^2}\int_0^x\zeta f(\zeta)d\zeta-\frac x3\int_x^\infty\frac{f(\zeta)}{\zeta^2}d\zeta.}
$$

For bounded forcing these integrals converge and give a bounded solution. It is unique because no nonzero combination of $x,x^{-2}$ is bounded at both ends. For a more general forcing, convergence and boundedness of the displayed integral must be checked.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
