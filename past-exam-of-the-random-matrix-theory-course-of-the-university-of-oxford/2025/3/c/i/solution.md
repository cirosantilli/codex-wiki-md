<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [characteristic function](../../../../../characteristic-function-split.md) of $B(t)\sim N(0,t)$ gives $\mathbb E e^{2iB(t)}=e^{-2t}$. Taking real parts and using $\sin^2b=(1-\cos2b)/2$,

$$
\boxed{\mathbb E\Delta(t)=\frac{1-e^{-2t}}2,
\qquad \lim_{t\to\infty}\mathbb E\Delta(t)=\frac12.}
$$

There is also a direct check from the [stochastic differential equation](../../../../../stochastic-differential-equation.md). Its [Itô integral](../../../../../ito-integral.md) has zero [expectation](../../../../../expected-value-split.md) because its integrand is bounded. Thus $m(t)=\mathbb E\Delta(t)$ satisfies $m'(t)=1-2m(t)$ and $m(0)=0$, whose solution is the same expression.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
