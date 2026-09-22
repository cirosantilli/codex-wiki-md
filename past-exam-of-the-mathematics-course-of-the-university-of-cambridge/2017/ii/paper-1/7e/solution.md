<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

There is an important convention issue in the printed statement. The ordinary [Cauchy principal value](../../../../../cauchy-principal-value.md) exists only for $n=1$. Closing the Fourier contour in the lower half-plane, with a small indentation above the real-axis pole, gives

$$
\boxed{\operatorname{PV}\int_{\mathbb R}\frac{e^{-ix}}x\,dx=-i\pi}.
$$

Equivalently, the odd cosine contribution cancels and the [Dirichlet integral](../../../../../dirichlet-integral.md) $\int_0^\infty\sin x/x\,dx=\pi/2$ supplies the imaginary part.

For $n\ge2$, the paired integrand near zero is $2\cos x/x^n$ if $n$ is even and $-2i\sin x/x^n$ if $n$ is odd. Its leading even power is nonintegrable: $x^{-n}$ in the first case and $x^{1-n}$ in the second. Thus **the ordinary principal value diverges for every $n>1$**.

If the intended convention is the [Hadamard finite-part integral](../../../../../hadamard-finite-part-integral.md), define it consistently by distributional differentiation,

$$
\operatorname{Pf}\frac1{x^n}
=\frac{(-1)^{n-1}}{(n-1)!}\frac{d^{n-1}}{dx^{n-1}}\operatorname{PV}\frac1x.
$$

Integration by parts in this distributional pairing, or regularized Fourier transformation, then gives

$$
\boxed{\operatorname{Pf}\int_{\mathbb R}\frac{e^{-ix}}{x^n}\,dx
=\frac{\pi(-i)^n}{(n-1)!}}.
$$

The distinction is essential: subtracting the divergent local Taylor terms supplies a finite part, but symmetric exclusion alone does not.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
