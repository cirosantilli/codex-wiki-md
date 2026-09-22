<h1 id="17/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [homogeneous first-order differential equation](../../../../../../homogeneous-first-order-differential-equation.md) suggests $v=y/x$, so $y'=v+xv'$. Wherever the original equation is defined,

$$
xv'=-\tan v,\qquad\frac{d}{dx}[x\sin v]=\sin v+x\cos v\,v'=0.
$$

Thus the implicit solution is $x\sin(y/x)=C$. The printed initial values force $C=x_0=2/\pi$.

**There is no classical solution through the printed initial point.** There $y/x=\pi/2$, so the tangent on the right is undefined. The implicit relation nevertheless has two neighboring real branches on $x>x_0$ which approach that point continuously:

$$
\boxed{y_1(x)=x\arcsin(x_0/x),\qquad y_2(x)=x[\pi-\arcsin(x_0/x)],\quad x_0=2/\pi.}
$$

Both tend to $y=1$ as $x\downarrow x_0$, but their [derivatives](../../../../../../derivative.md) become unbounded with opposite signs. They solve the equation on the open interval $x>x_0$, not at its endpoint. Other inverse-sine periods cannot approach the specified initial value. This is an [endpoint obstruction in a homogeneous differential equation](../../../../../../endpoint-obstruction-in-a-homogeneous-differential-equation.md). Constant-ratio branches $y=k\pi x$ also solve the general equation where $x\ne0$, but do not meet the initial data.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [17](../../../17.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
