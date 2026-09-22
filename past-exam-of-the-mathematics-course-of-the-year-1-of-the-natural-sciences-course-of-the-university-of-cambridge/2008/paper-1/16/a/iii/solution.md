<h1 id="16/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

On an interval avoiding zero put $v=y/x$. A real solution requires $|v|\leq1$, and the principal [square root](../../../../../../square-root.md) is $\sqrt{x^2-y^2}=|x|\sqrt{1-v^2}$. The [homogeneous first-order differential equation](../../../../../../homogeneous-first-order-differential-equation.md) reduces to

$$
v'=\frac{\sqrt{1-v^2}}{|x|}.
$$

Where $|v|<1$, [separation of variables](../../../../../../separation-of-variables.md) gives $\arcsin v=\operatorname{sgn}(x)\log|x|+C$. Thus the nonconstant pieces are

$$
\boxed{y=x\sin\bigl(\operatorname{sgn}(x)\log|x|+C\bigr),}
$$

restricted to intervals where the cosine of the phase is nonnegative. This sign condition is essential when substituting back into the original [square root](../../../../../../square-root.md).

There are also the solutions $y=x$ and $y=-x$. They can join the nonconstant pieces with a continuous first [derivative](../../../../../../derivative.md), because the transformed rate vanishes but is not [Lipschitz continuous](../../../../../../lipschitz-continuity.md) at $v=\pm1$. For example, on the positive axis every $A>0$ gives

$$
y(x)=\begin{cases}-x,&0<x\leq A,\\x\sin\bigl(\log(x/A)-\pi/2\bigr),&A<x<Ae^\pi,\\x,&x\geq Ae^\pi.\end{cases}
$$

The [sticking solutions of a bounded square-root differential equation](../../../../../../sticking-solutions-of-a-bounded-square-root-differential-equation.md) describe the same joining mechanism on either half-axis after using the increasing variable $t=\operatorname{sgn}(x)\log|x|$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [16](../../../16.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
