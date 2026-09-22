<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The complete integral is $\Gamma(1/2)=\sqrt\pi$. Therefore apply [asymptotic expansion by repeated integration by parts](../../../../../../asymptotic-expansion-by-repeated-integration-by-parts.md) to the tail $I(x)=\int_x^\infty t^{-1/2}e^{-t}\,dt$:

$$
I(x)=e^{-x}x^{-1/2}-\frac12\int_x^\infty t^{-3/2}e^{-t}\,dt
=e^{-x}\left(x^{-1/2}-\frac12x^{-3/2}+\frac34x^{-5/2}\right)-\frac{15}8\int_x^\infty t^{-7/2}e^{-t}\,dt.
$$

The last integral is bounded by $x^{-7/2}e^{-x}$. Thus

$$
\boxed{f(x)=\sqrt\pi-e^{-x}x^{-1/2}+\tfrac12e^{-x}x^{-3/2}-\tfrac34e^{-x}x^{-5/2}+O(e^{-x}x^{-7/2}).}
$$

In particular the first three additive terms are $\sqrt\pi$, $-e^{-x}x^{-1/2}$ and $\tfrac12e^{-x}x^{-3/2}$; the formula also supplies three successive terms of the exponentially small tail if the constant is counted separately. A power expansion alone would retain only $\sqrt\pi$ and miss this information.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
