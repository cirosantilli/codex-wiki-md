<h1 id="differential-equations/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

First solve for $v=y'$. [Multiplication](../../../../multiplication.md) by $e^x$ and use of $v(1)=0$ give

$$
v(x)=-e^{-x}\int_x^1e^tf(t)\,dt.
$$

Integrating from zero to $x$, and using $y(0)=0$, yields $y(x)=-\int_0^xe^{-s}\int_s^1e^tf(t)\,dt\,ds$. Reversing the order of integration gives

$$
\boxed{G_1(x,t)=1-e^t\quad(0\leq t\leq x),\qquad G_2(x,t)=e^{t-x}-e^t\quad(x\leq t\leq1).}
$$

Thus $G(x,t)$ equals $G_1$ for $t<x$ and $G_2$ for $x<t$. It is continuous at $x=t$, vanishes at $x=0$, and has $G_x(1,t)=0$. Its derivative jumps from $-1$ to zero across $x=t$, so the jump is $+1$, matching the coefficient of $y''$. Both pieces satisfy $G_{xx}+G_x=0$ away from the jump. These facts also verify the Green representation directly. The homogeneous solutions are $A+Be^{-x}$, and the two [boundary conditions](../../../../boundary-condition.md) force $A=B=0$, proving [uniqueness](../../../../uniqueness.md).

For $f(t)=e^{-t}$, the formula gives

$$
\int_0^x(e^{-t}-1)\,dt+\int_x^1(e^{-x}-1)\,dt=-xe^{-x}.
$$

Hence **$y(x)=-xe^{-x}$**. Indeed $y'=(x-1)e^{-x}$ and $y''=(2-x)e^{-x}$, which verify the equation and both [boundary conditions](../../../../boundary-condition.md).

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Differential equations](../../differential-equations.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
