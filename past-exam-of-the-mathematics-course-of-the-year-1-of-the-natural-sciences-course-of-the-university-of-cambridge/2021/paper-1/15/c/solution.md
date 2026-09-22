<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x>0$, the definition of [hyperbolic cosine](../../../../../hyperbolic-cosine.md) simplifies the composite function exactly:

$$
\cosh(\ln x)=\frac{e^{\ln x}+e^{-\ln x}}2=\frac12\left(x+\frac1x\right).
$$

Let $h=x-2$. The [geometric series](../../../../../geometric-series.md) gives

$$
\frac1{2+h}=\frac12\left(1-\frac h2+\frac{h^2}4-\frac{h^3}8+O(h^4)\right).
$$

Adding $2+h$ and dividing by two gives the requested [Taylor expansion](../../../../../taylor-expansion.md):

$$
\boxed{\cosh(\ln x)=\frac54+\frac38(x-2)+\frac1{16}(x-2)^2-\frac1{32}(x-2)^3+O((x-2)^4).}
$$

The underlying infinite geometric expansion has $|x-2|<2$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
