<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The parameter [derivative](../../../../../derivative.md) of the integrand is $\cos(a\log x)$, whose absolute value is bounded by one on $0<x<1$. This integrable bound justifies [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md), giving

$$
I'(a)=\int_0^1\cos(a\log x)\,dx.
$$

The original [integral](../../../../../integral-split.md) also exists: $|\sin(a\log x)/\log x|\leq|a|$, and its apparent singularity at $x=1$ is removable. Set $x=e^{-t}$ to evaluate the [derivative](../../../../../derivative.md):

$$
I'(a)=\int_0^\infty e^{-t}\cos(at)\,dt
=\operatorname{Re}\int_0^\infty e^{-(1-ia)t}\,dt
=\operatorname{Re}\frac1{1-ia}.
$$

Consequently

$$
\boxed{I'(a)=\frac1{1+a^2}}.
$$

Since $I(0)=0$, integration in the parameter fixes the constant and gives the [logarithmic sine integral](../../../../../logarithmic-sine-integral.md) identity

$$
\boxed{I(a)=\arctan a,\qquad I(1)=\frac\pi4}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
