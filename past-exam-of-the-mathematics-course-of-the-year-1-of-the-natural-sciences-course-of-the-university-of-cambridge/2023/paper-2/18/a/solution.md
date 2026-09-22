<h1 id="18/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $I_n=\int\sin^nx\,dx$. Apply [integration by parts](../../../../../integration-by-parts.md) with $\sin^{n-1}x$ and $\sin x\,dx$:

$$
I_n=-\cos x\sin^{n-1}x+(n-1)\int\sin^{n-2}x\cos^2x\,dx.
$$

Using $\cos^2x=1-\sin^2x$ on the right gives $I_n=-\cos x\sin^{n-1}x+(n-1)(I_{n-2}-I_n)$. Rearranging proves

$$
\boxed{I_n=-\frac{\cos x\sin^{n-1}x}{n}+\frac{n-1}{n}I_{n-2}+C}.
$$

For $J_n=\int\cos^nx\,dx$, the analogous [integration by parts](../../../../../integration-by-parts.md) uses $\cos^{n-1}x$ and $\cos x\,dx$, giving $J_n=\sin x\cos^{n-1}x+(n-1)(J_{n-2}-J_n)$. Hence

$$
\boxed{J_n=\frac{\sin x\cos^{n-1}x}{n}+\frac{n-1}{n}J_{n-2}+C}.
$$

An arbitrary [constant of integration](../../../../../constant-of-integration.md) absorbs the choices in the lower-order [antiderivatives](../../../../../antiderivative.md).

Starting from $I_0=J_0=x$, successive use of $n=2,4,6$ gives

$$
\boxed{\int\sin^6x\,dx=
\frac{5x}{16}-\frac{\cos x\sin^5x}{6}
-\frac{5\cos x\sin^3x}{24}-\frac{5\sin x\cos x}{16}+C},
$$



$$
\boxed{\int\cos^6x\,dx=
\frac{5x}{16}+\frac{\sin x\cos^5x}{6}
+\frac{5\sin x\cos^3x}{24}+\frac{5\sin x\cos x}{16}+C}.
$$

These expressions follow directly from the requested recurrence, rather than requiring a separate trigonometric expansion.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
