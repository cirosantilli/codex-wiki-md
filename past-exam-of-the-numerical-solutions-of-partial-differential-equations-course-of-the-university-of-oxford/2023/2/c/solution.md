<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $z=\pi h/2$, so $0<z\leq\pi/4$. The formulas in (a) and (b) give

$$
\lambda_{1,1}-\Lambda_{1,1}=\frac8{h^2}(z^2-\sin^2z).
$$

For $0\leq t\leq\pi/4$, $0\leq\sin t\leq t$ and $1-\cos t=2\sin^2(t/2)\leq t^2/2$. Therefore

$$
0\leq z-\sin z=\int_0^z(1-\cos t)dt\leq\frac{z^3}6.
$$

These [trigonometric inequalities](../../../../trigonometric-inequality.md) imply

$$
0\leq z^2-\sin^2z=(z-\sin z)(z+\sin z)\leq\frac{z^3}6(2z)=\frac{z^4}3.
$$

Substitution yields the explicit [eigenvalue](../../../../eigenvalue.md) error bound

$$
\boxed{|\lambda_{1,1}-\Lambda_{1,1}|\leq\frac{\pi^4}{6}h^2,\qquad C=\frac{\pi^4}{6}.}
$$

This constant is asymptotically sharp: [Taylor's theorem](../../../../taylor-s-theorem.md) gives $\sin^2z=z^2-z^4/3+O(z^6)$, so $(\lambda_{1,1}-\Lambda_{1,1})/h^2\to\pi^4/6$. Here $O$ denotes [Big O notation](../../../../big-o-notation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
