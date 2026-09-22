<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u=x^{-5}$, which tends to zero as $|x|\to\infty$. Factor the denominator and use the [cosecant expansion near zero](../../../../../cosecant-expansion-near-zero.md):

$$
g(x)=x^2\frac{u}{\sin u},\qquad
\frac{u}{\sin u}=\left(1-\frac{u^2}{6}+\frac{u^4}{120}+O(u^6)\right)^{-1}
=1+\frac{u^2}{6}+\frac{7u^4}{360}+O(u^6).
$$

Substitution gives the first two nonzero terms and the requested omitted order:

$$
\boxed{g(x)=x^2+\frac1{6x^8}+O(x^{-18}),\qquad |x|\to\infty.}
$$

More precisely the next term is $7/(360x^{18})$, followed by $O(x^{-28})$. The outside factor $x^2$ is essential when converting the remainder order from powers of $u$ to powers of $x$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
