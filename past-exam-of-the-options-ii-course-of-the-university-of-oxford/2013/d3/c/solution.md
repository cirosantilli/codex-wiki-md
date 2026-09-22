<h1 id="d3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $0<x<1$, the geometric expansion gives summands $h_n(x)=x^{n+\beta-1}-x^{n-\beta}$. Their [integrals](../../../../integral-split.md) are

$$
\int_0^1h_n(x)\,dx
=\frac1{n+\beta}-\frac1{n+1-\beta}
=\frac{1-2\beta}{n^2+n+\beta-\beta^2}.
$$

Both powers are integrable because $0<\beta<1$. If $\beta<1/2$, each $h_n$ is nonnegative, since its first exponent is smaller. Their [integrals](../../../../integral-split.md) form a convergent nonnegative series: the $n=0$ term is finite and subsequent terms are bounded by a constant times $n^{-2}$. The proved series-integration rule applies.

If $\beta>1/2$, apply precisely that rule to $-h_n$, which are nonnegative, and negate the result. At $\beta=1/2$ all summands and the integrand are zero. Thus in every case the [integral](../../../../integral-split.md) is absolutely integrable and

$$
\boxed{\int_0^1\frac{x^{\beta-1}-x^{-\beta}}{1-x}\,dx
=\sum_{n=0}^{\infty}\frac{1-2\beta}{n^2+n+\beta-\beta^2}.}
$$

The common sign of the summands is the reason no unproved theorem for integrating arbitrary signed series is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [D3](../../d3.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
