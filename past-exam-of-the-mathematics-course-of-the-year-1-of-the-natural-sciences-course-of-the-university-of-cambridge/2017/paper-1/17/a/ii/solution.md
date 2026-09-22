<h1 id="17/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Separate one factor of the [hyperbolic sine](../../../../../../hyperbolic-sine.md) and use the [hyperbolic Pythagorean identity](../../../../../../hyperbolic-pythagorean-identity.md) $\sinh^2x=\cosh^2x-1$. With $u=\cosh x$ and $du=\sinh x\,dx$, [integration by substitution](../../../../../../integration-by-substitution.md) gives

$$
\int\frac{\sinh^3x}{\cosh^2x}\,dx
=\int\frac{u^2-1}{u^2}\,du
=\int(1-u^{-2})\,du
=\boxed{\cosh x+\frac1{\cosh x}+C}.
$$

For real $x$, the [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) never vanishes. Differentiating the result gives $\sinh x(1-\operatorname{sech}^2x)=\sinh^3x/\cosh^2x$, checking the sign of the reciprocal term.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [17](../../../17.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
