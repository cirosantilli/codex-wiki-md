<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $m>-1$, integrate the base [power](../../../../../power.md) to obtain $J(m)=\int_0^1x^m\,dx=1/(m+1)$. Since $\partial_m^n x^m=x^m(\log x)^n$, differentiating $n$ times gives

$$
\boxed{\int_0^1x^m(\log x)^n\,dx
=\frac{d^n}{dm^n}\frac1{m+1}
=\frac{(-1)^nn!}{(m+1)^{n+1}}}.
$$

Here $n$ is a nonnegative integer. For justification, keep $m$ in a small closed interval bounded below by $m_0>-1$. The differentiated integrands are dominated by $x^{m_0}|\log x|^n$, whose [integral](../../../../../integral-split.md) becomes $\int_0^\infty e^{-(m_0+1)t}t^n\,dt$ under $x=e^{-t}$ and is finite. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) establishes the needed [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) and the [logarithmic moments of a power on the unit interval](../../../../../logarithmic-moments-of-a-power-on-the-unit-interval.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
