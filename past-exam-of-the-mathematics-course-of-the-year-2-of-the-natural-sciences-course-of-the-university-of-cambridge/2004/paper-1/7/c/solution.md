<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [drift-removing substitution for a Dirichlet Sturm-Liouville problem](../../../../../drift-removing-substitution-for-a-dirichlet-sturm-liouville-problem.md), $z(x)=e^{-2x}u(x)$. It gives $u''+\lambda u=0$ with $u(0)=u(1)=0$. Positive $\lambda=k^2$ requires $\sin k=0$; zero or negative $\lambda$ yields only the trivial solution under both endpoint conditions. Hence

$$
\boxed{\lambda_n=n^2\pi^2,\qquad z_n(x)=e^{-2x}\sin(n\pi x),\qquad n=1,2,\ldots.}
$$

Multiplication of the original equation by $e^{4x}$ gives $-(e^{4x}z')'-4e^{4x}z=\lambda e^{4x}z$. Thus the appropriate [weighted inner product](../../../../../weighted-inner-product.md) has weight $e^{4x}$, and

$$
\boxed{\int_0^1e^{4x}z_m(x)z_n(x)dx=\int_0^1\sin(m\pi x)\sin(n\pi x)dx=\frac12\delta_{mn}.}
$$

Multiplying each eigenfunction by $\sqrt2$ gives weighted norm one.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
