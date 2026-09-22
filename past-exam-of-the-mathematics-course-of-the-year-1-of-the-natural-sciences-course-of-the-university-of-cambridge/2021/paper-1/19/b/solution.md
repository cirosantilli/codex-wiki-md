<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor out the dominant cubic term and use a [geometric series](../../../../../geometric-series.md) in $1/(3x^2)$:

$$
\frac1{x+3x^3}=\frac1{3x^3}\left(1+\frac1{3x^2}\right)^{-1}=\frac1{3x^3}-\frac1{9x^5}+O(x^{-7}).
$$

Thus the requested leading term and absolute error order are

$$
\boxed{g(x)=\frac1{3x^3}+O(x^{-5})\qquad(x\to+\infty).}
$$

The relative error of retaining only the leading term is $O(x^{-2})$; it differs from the absolute error order $O(x^{-5})$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
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
