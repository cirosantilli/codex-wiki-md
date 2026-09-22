<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n>1$, [integration by parts](../../../../../integration-by-parts.md) with $u=x^{n-1}$ and $dv=e^{-x}\,dx$ yields

$$
I_n=[-x^{n-1}e^{-x}]_0^\infty+(n-1)\int_0^\infty x^{n-2}e^{-x}\,dx=(n-1)I_{n-1}.
$$

The boundary term vanishes at zero because $n-1>0$, and at infinity because exponential decay dominates every fixed power. The initial [improper integral](../../../../../improper-integral.md) is $I_1=\int_0^\infty e^{-x}\,dx=1$. Iterating the [recurrence relation](../../../../../recurrence-relation.md) therefore gives

$$
\boxed{I_n=(n-1)(n-2)\cdots1\,I_1=(n-1)!,\qquad n\ge1.}
$$

This is the positive-integer case of the [Gamma function](../../../../../gamma-function.md) identity $\Gamma(n)=(n-1)!$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
