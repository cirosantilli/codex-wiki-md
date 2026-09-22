<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $f(x)=x^{1/3}$, the required [derivatives](../../../../../derivative.md) are

$$
f'(x)=\frac13x^{-2/3},\quad f''(x)=-\frac29x^{-5/3},\quad
f^{(3)}(x)=\frac{10}{27}x^{-8/3}.
$$

At $a=8$ these give $f(8)=2$, $f'(8)=1/12$, and $f''(8)=-1/144$. Setting $x-a=1$, the three-term [Taylor polynomial](../../../../../taylor-polynomial.md) yields

$$
\boxed{9^{1/3}\approx2+\frac1{12}-\frac1{288}=\frac{599}{288}\approx2.07986111.}
$$

By the [Taylor theorem with Lagrange remainder](../../../../../taylor-theorem-with-lagrange-remainder.md), the signed error is

$$
R_3=\frac{f^{(3)}(\xi)}{6}=\frac5{81}\xi^{-8/3},\qquad 8<\xi<9.
$$

It is positive, and $\xi^{-8/3}<8^{-8/3}=1/256$. Consequently

$$
\boxed{0<9^{1/3}-\frac{599}{288}<\frac5{20736}<\frac1{4000}.}
$$

The last comparison is exact because $5\cdot4000=20000<20736$. Thus the estimate is an underestimate with the required rigorous [absolute error](../../../../../absolute-error.md) bound.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
