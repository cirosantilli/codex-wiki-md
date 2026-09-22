<h1 id="18/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the [inner product](../../../../../../inner-product-split.md) of the [Fourier series](../../../../../../fourier-series-split.md) with $\sin(n\pi x/L)$. [Fourier orthogonality](../../../../../../fourier-orthogonality.md) eliminates the constant, all cosine terms, and all sine terms except the $n$th. The remaining squared [norm](../../../../../../norm.md) is

$$
\int_{-L}^{L}\sin^2(n\pi x/L)\,dx=L,
$$

so

$$
\boxed{b_n=\frac1L\int_{-L}^{L}f(x)\sin(n\pi x/L)\,dx,\qquad n\geq1}.
$$

For a [square-integrable function](../../../../../../square-integrable-function.md), the calculation is justified by taking [inner products](../../../../../../inner-product-split.md) of finite [Fourier partial sums](../../../../../../fourier-partial-sum.md) and passing to their [mean-square limit](../../../../../../convergence-in-l2.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
