<h1 id="8/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Write $P_n(x)\sim c_nx^n$ with $c_n\ne0$. For $n\geq1$, this branch grows. Choosing the other [reduction of order](../../../../../reduction-of-order.md) solution by an integral from infinity gives, on $x>1$,

$$
P_n(x)\int_\infty^x\frac{dt}{(1-t^2)P_n(t)^2}\sim\frac{x^{-n-1}}{c_n(2n+1)}.
$$

Thus **for $n\geq1$, every bounded exterior solution decays as $|x|^{-n-1}$**, up to a constant factor, on each exterior interval. Equivalently the dominant-balance exponents in the [Legendre differential equation](../../../../../legendre-differential-equation.md) are $n$ and $-n-1$.

There is an important exception at degree zero. Since $P_0=1$,

$$
\boxed{y=C_1+\frac{C_2}{2}\log\left|\frac{x+1}{x-1}\right|=C_1+\frac{C_2}{x}+O(|x|^{-3})\quad(n=0).}
$$

These solutions are bounded even when $C_1\ne0$; boundedness alone does not then imply decay to zero. The constants on $x>1$ and $x<-1$ are independent unless continuation across the singular endpoints is specified.

## ↑ Ancestors (13)

1. [Vi](../vi.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
