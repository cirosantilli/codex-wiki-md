<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n>1$, the [Taylor series](../../../../../taylor-series.md) of the [natural logarithm](../../../../../natural-logarithm.md) converges absolutely at $1/n$:

$$
\ln\left(1+\frac1n\right)=\sum_{j=1}^{\infty}\frac{(-1)^{j+1}}{jn^j}.
$$

Multiply this [power series](../../../../../power-series.md) by $n+1/2$ and subtract $1$. The constant term cancels the subtracted $1$, and the coefficient of $1/n$ is $-1/2+1/2=0$. For $k\geq2$, the coefficient of $n^{-k}$ is

$$
\frac{(-1)^k}{k+1}+\frac{(-1)^{k+1}}{2k}=(-1)^k\left(\frac1{k+1}-\frac1{2k}\right).
$$

Hence

$$
\boxed{u_n=\sum_{k=2}^{\infty}\frac{(-1)^k}{n^k}\left(\frac1{k+1}-\frac1{2k}\right).}
$$

In particular $u_n=1/(12n^2)-1/(12n^3)+O(n^{-4})$, in [Big O notation](../../../../../big-o-notation.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
