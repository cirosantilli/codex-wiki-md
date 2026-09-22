<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [power series](../../../../../power-series.md) of the [exponential function](../../../../../exponential-function.md):

$$
\frac{e^{-x^2}}{\sqrt x}=\sum_{n=0}^\infty a_n(x),\qquad
a_n(x)=\frac{(-1)^n x^{2n-1/2}}{n!},\quad0<x<1.
$$

Each term is a [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md), and

$$
\int_0^1|a_n(x)|\,dx
=\frac{1}{n!(2n+1/2)}=\frac{2}{(4n+1)n!}.
$$

The sum of these nonnegative integrals is at most $2\sum_{n\geq0}1/n!=2e<\infty$. Applying [integration of a series with summable L1 norms](../../../../../integration-of-a-series-with-summable-l1-norms.md), just proved in part (ii), therefore justifies exchanging the series and the integral:

$$
\boxed{\int_0^1\frac{e^{-x^2}}{\sqrt x}\,dx
=2\sum_{n=0}^\infty\frac{(-1)^n}{(4n+1)n!}.}
$$

The absolute-integral bound is the justification; pointwise convergence of the exponential series alone would not suffice.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
