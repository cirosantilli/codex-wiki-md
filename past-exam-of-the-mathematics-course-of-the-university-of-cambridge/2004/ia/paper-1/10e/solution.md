<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

Use [integration by parts](../../../../../integration-by-parts.md) on $\sin^{n-1}x\sin x$, for $n\geq2$:

$$
\begin{aligned}
I_n
&=[-\sin^{n-1}x\cos x]_0^{\pi/2}
+(n-1)\int_0^{\pi/2}\sin^{n-2}x\cos^2x\,dx\\
&=(n-1)(I_{n-2}-I_n).
\end{aligned}
$$

Both boundary terms are zero. Therefore the [Wallis integrals](../../../../../wallis-integrals.md) satisfy

$$
\boxed{nI_n=(n-1)I_{n-2}.}
$$

Starting with $I_0=\pi/2$ and $I_1=1$, repeated application gives

$$
\begin{aligned}
I_{2n}&=\frac{1\cdot3\cdots(2n-1)}{2\cdot4\cdots2n}\frac\pi2
=\frac{(2n)!}{2^{2n}(n!)^2}\frac\pi2,\\
I_{2n+1}&=\frac{2\cdot4\cdots2n}{3\cdot5\cdots(2n+1)}
=\frac{2^{2n}(n!)^2}{(2n+1)!}.
\end{aligned}
$$

These formulas also hold at $n=0$ by empty products.

For $0<x<\pi/2$, $0<\sin x<1$, so $0<\sin^n x<\sin^{n-1}x$ when $n\geq1$. Integrating the strict inequalities proves $0<I_n<I_{n-1}$. In particular $I_{2n+1}/I_{2n}<1$. For $n\geq1$, the recurrence and $I_{2n-1}>I_{2n}$ give

$$
I_{2n+1}=\frac{2n}{2n+1}I_{2n-1}
>\frac{2n}{2n+1}I_{2n}.
$$

Thus

$$
\boxed{\frac{2n}{2n+1}<\frac{I_{2n+1}}{I_{2n}}<1.}
$$

At $n=0$ the same displayed bounds are $0<2/\pi<1$, also true directly from $I_1<I_0$.

The [squeeze theorem](../../../../../squeeze-theorem.md) now gives $I_{2n+1}/I_{2n}\to1$. Substituting the evaluated integrals shows

$$
\frac{I_{2n+1}}{I_{2n}}
=\frac1\pi\frac{2^{4n+1}(n!)^4}{(2n+1)((2n)!)^2},
$$

and hence

$$
\boxed{\lim_{n\to\infty}\frac{2^{4n+1}(n!)^4}{(2n+1)((2n)!)^2}=\pi.}
$$

This is twice the finite-product form of the [Wallis product](../../../../../wallis-product.md); the proof used only the integral recurrence and strict comparison of its integrands.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
