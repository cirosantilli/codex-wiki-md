<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

For $0<a<2$, the beta-integral evaluation gives

$$
I(a)=\int_0^\infty\frac{x^{a-1}}{1+x^2}\,dx
=\frac\pi2\csc\frac{\pi a}{2}.
$$

[Differentiation](../../../../../differentiation.md) under the [integral](../../../../../integral.md) sign near $a=1$ is justified by domination at zero and infinity. Therefore

$$
I^{(4)}(1)=\int_0^\infty\frac{(\log x)^4}{1+x^2}\,dx.
$$

Writing $a=1+t$ gives

$$
I(1+t)=\frac\pi2\sec\frac{\pi t}{2}.
$$

Since

$$
\sec z=1+\frac{z^2}{2}+\frac{5z^4}{24}+O(z^6),
$$

the [logarithmic moments of the Cauchy kernel](../../../../../logarithmic-moments-of-the-cauchy-kernel.md) yield

$$
\boxed{
\int_0^\infty\frac{(\log x)^4}{1+x^2}\,dx
=\frac{5\pi^5}{32}}.
$$

The same expansion gives $I''(1)=\pi^3/8$, agreeing with the supplied identity.

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
