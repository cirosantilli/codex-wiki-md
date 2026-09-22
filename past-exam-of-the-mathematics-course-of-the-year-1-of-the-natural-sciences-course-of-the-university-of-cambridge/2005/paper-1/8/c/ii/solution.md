<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $x>0$ and $\alpha>1$, the preceding antiderivative gives

$$
\frac{\operatorname{sech}x-\operatorname{sech}(\alpha x)}x=\int_1^\alpha\operatorname{sech}(xy)\tanh(xy)\,dy.
$$

The integrand is nonnegative, so [Tonelli's theorem](../../../../../../tonelli-theorem.md) permits reversing the two integrals without first assuming absolute integrability. Put $u=xy$ in the inner integral to obtain the [hyperbolic-secant Frullani integral](../../../../../../hyperbolic-secant-frullani-integral.md):

$$
I=\int_1^\alpha\frac{dy}{y}\int_0^\infty\operatorname{sech}u\tanh u\,du=\int_1^\alpha\frac{dy}{y}=\boxed{\ln\alpha}.
$$

Here $\int_0^\infty\operatorname{sech}u\tanh u\,du=[-\operatorname{sech}u]_0^\infty=1$. Near zero, cancellation makes the original integrand $O(x)$; at infinity it decays exponentially. The finite result therefore also establishes ordinary convergence of the [improper integral](../../../../../../improper-integral.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
