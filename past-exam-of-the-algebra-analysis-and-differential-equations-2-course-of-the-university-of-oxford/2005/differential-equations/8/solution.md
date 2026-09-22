<h1 id="differential-equations/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Put

$$
z(x)=-\int_0^x\sin(x-s)f(s)\,ds.
$$

Leibniz differentiation gives $z'=-\int_0^x\cos(x-s)f(s)\,ds$ and $z''=-f(x)+\int_0^x\sin(x-s)f(s)\,ds=-f-z$. Thus $z$ satisfies both [zero](../../../../zero-of-a-function.md) [initial conditions](../../../../initial-condition.md) and the inhomogeneous equation. Every solution with $y(0)=0$ is $y=A\sin x+z(x)$.

On $[0,1]$, the second endpoint determines $A=-z(1)/\sin1$ uniquely, since $\sin1\ne0$. Collecting the integrals, and using the [sine addition formula](../../../../sine-addition-formula.md) for $s<x$, gives

$$
\boxed{G(x,s)=\frac{\sin(\min\{x,s\})\sin(1-\max\{x,s\})}{\sin1}.}
$$

This continuous kernel vanishes at the endpoints, satisfies $G_{xx}+G=0$ off $x=s$, and has derivative jump $-1$, as required for $-y''-y=f$. The preceding construction proves existence, and a homogeneous solution with both endpoints [zero](../../../../zero-of-a-function.md) must vanish, proving uniqueness.

On $[0,\pi]$, instead, the second boundary value becomes

$$
y(\pi)=z(\pi)=-\int_0^\pi f(s)\sin s\,ds.
$$

Thus **solvability is equivalent to $\int_0^\pi f(s)\sin s\,ds=0$**. When it holds, all solutions are

$$
\boxed{y(x)=A\sin x-\int_0^x\sin(x-s)f(s)\,ds,\qquad A\in\mathbb R.}
$$

There is one free homogeneous mode because the endpoint length is resonant.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Differential equations](../../differential-equations.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
