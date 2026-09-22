<h1 id="15/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating first over $z$ multiplies by $e^y$. Split at $y=0$ to handle the [absolute value](../../../../../../absolute-value.md) correctly:

$$
J=\int_0^1x\left[\int_{-x/2}^0(-y)e^y\,dy+\int_0^xy e^y\,dy\right]dx.
$$

[Integration by parts](../../../../../../integration-by-parts.md) gives [antiderivatives](../../../../../../antiderivative.md) $(1-y)e^y$ and $(y-1)e^y$ for these two inner [integrands](../../../../../../integrand.md). Their contributions are

$$
1-(1+x/2)e^{-x/2},\qquad (x-1)e^x+1,
$$

respectively. Thus

$$
J=\int_0^1\left[2x+(x^2-x)e^x-(x+x^2/2)e^{-x/2}\right]dx.
$$

For the remaining [integrals](../../../../../../integral-split.md),

$$
\int_0^1(x^2-x)e^x\,dx
=\left[e^x(x^2-3x+3)\right]_0^1=e-3,
$$

and

$$
\int_0^1(x+x^2/2)e^{-x/2}\,dx
=\left[-e^{-x/2}(x^2+6x+12)\right]_0^1
=12-19e^{-1/2}.
$$

Combining them yields

$$
\boxed{J=e-14+19e^{-1/2}}.
$$

The upper $z$ bound is $e^y$, as in the original PDF; an additional truncated version in the OCR must not be used.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [15](../../../15.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
