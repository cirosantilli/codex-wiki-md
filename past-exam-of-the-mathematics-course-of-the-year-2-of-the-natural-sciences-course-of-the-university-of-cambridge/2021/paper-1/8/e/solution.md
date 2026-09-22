<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Taylor series](../../../../../taylor-series.md) of the logarithm gives

$$
\log(1+x)=\sum_{j=1}^\infty\frac{(-1)^{j+1}}j x^j=x\sum_{k=0}^\infty\frac{(-x)^k}{k+1}.
$$

Therefore the closed form of the larger-root [Frobenius solution](../../../../../frobenius-solution.md) is

$$
\boxed{y(x)=a_0\sqrt{x}\log(1+x).}
$$

The series derivation holds initially for $0<x<1$; the closed form extends as a real solution to all $x>0$. To check it without series, put $y=\sqrt{x}\,v(x)$ in the original equation. All undifferentiated $v$ terms cancel and the remaining expression is $4x^{5/2}[(1+x)v''+v']$. Hence $[(1+x)v']'=0$, and $v=\log(1+x)$ indeed solves it. Its logarithm is analytic near zero, so this is not a forced $\log x$ companion term at the Frobenius point.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
