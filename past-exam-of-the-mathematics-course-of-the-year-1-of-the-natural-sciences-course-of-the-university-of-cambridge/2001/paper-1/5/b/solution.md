<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $u=1/x$, so $dx=-du/u^2$ and $\ln x=-\ln u$. Reversing the integration bounds gives, without evaluating either side,

$$
\boxed{\int_1^\infty\frac{\ln x}{x^2}dx=-\int_0^1\ln u\,du.}
$$

For $J=\int_0^\infty\ln x/(1+x^2)dx$, the same [change of variables](../../../../../change-of-variables-formula.md) gives

$$
J=-\int_0^\infty\frac{\ln u}{1+u^2}du=-J,
$$

so $\boxed{J=0}$. These are legitimate transformations of [improper integrals](../../../../../improper-integral.md): $|\ln x|$ is integrable near zero, and $(\ln x)/x^2$ is integrable at infinity. In particular $J$ is absolutely convergent, so no cancellation of divergent endpoints is being assumed.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
