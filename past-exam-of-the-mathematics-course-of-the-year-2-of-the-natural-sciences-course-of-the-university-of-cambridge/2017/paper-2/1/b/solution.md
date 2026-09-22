<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Projecting the [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) onto $y_m$ using the [weighted inner product](../../../../../weighted-inner-product.md) gives

$$
a_m=\langle f,y_m\rangle_w=\int_0^1w(x)f(x)y_m(x)\,dx.
$$

For the partial sum $f_N=\sum_{n=0}^Na_ny_n$, [orthonormality](../../../../../orthonormal-set.md) therefore gives

$$
\|f_N\|_w^2=\sum_{n,m=0}^Na_na_m\langle y_n,y_m\rangle_w=\sum_{n=0}^Na_n^2.
$$

For $f$ of finite [weighted norm](../../../../../weighted-norm.md), the given completeness means that $f_N\to f$ in that norm. The [triangle inequality](../../../../../triangle-inequality.md) implies $|\|f_N\|_w-\|f\|_w|\leq\|f_N-f\|_w\to0$. Taking the limit of the finite identity proves [Parseval's identity](../../../../../parseval-identity.md):

$$
\boxed{\int_0^1w(x)f(x)^2\,dx=\sum_{n=0}^\infty a_n^2.}
$$

This argument justifies the limiting step without assuming that a double infinite series can be integrated term by term. As usual, the expansion is understood for [square-integrable functions](../../../../../square-integrable-function.md) with respect to the weighted measure; the boundary and smoothness assumptions of the regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) provide the usual stronger interpretations when needed.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
