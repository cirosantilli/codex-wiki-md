<h1 id="16/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [expected value](../../../../../expected-value-split.md) is zero, so the [variance](../../../../../variance-split.md) is $\mathbb E[X^2]$. Symmetry gives

$$
\operatorname{Var}(X)=\frac2N\int_0^2x^2(1+e^{-x})\,dx.
$$

The polynomial term contributes $8/3$. Two applications of [integration by parts](../../../../../integration-by-parts.md) give

$$
\int x^2e^{-x}\,dx=-(x^2+2x+2)e^{-x}+C,
$$

so its definite value on $[0,2]$ is $2-10e^{-2}$. Therefore

$$
\boxed{\operatorname{Var}(X)=\frac{28/3-20e^{-2}}{6-2e^{-2}}.}
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
