<h1 id="question-4/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The [function](../../../../../../function-split.md) $x\sin(px)$ is an [even function](../../../../../../even-function.md), so every [Fourier sine coefficient](../../../../../../fourier-sine-coefficient.md) is zero. Introduce the auxiliary [integral](../../../../../../integral-split.md)

$$
I_k=\int_0^\pi x\sin(kx)\,dx.
$$

For a nonzero integer $k$, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
I_k=\left[-\frac{x\cos(kx)}k+\frac{\sin(kx)}{k^2}\right]_0^\pi
=-\frac{\pi(-1)^k}{k},\qquad I_0=0.
$$

Consequently

$$
a_0=\frac2\pi I_p=\frac{2(-1)^{p+1}}p.
$$

For $n\geq1$, a [product-to-sum formula](../../../../../../product-to-sum-formula.md) yields

$$
a_n=\frac1\pi(I_{p+n}+I_{p-n}).
$$

If $n\ne p$, this becomes

$$
a_n=-(-1)^{p+n}\left(\frac1{p+n}+\frac1{p-n}\right)
=\frac{2p(-1)^{p+n}}{n^2-p^2}.
$$

The exceptional [Fourier coefficient](../../../../../../fourier-coefficient.md) at $n=p$ must be evaluated before dividing by $p-n$:

$$
a_p=\frac1\pi(I_{2p}+I_0)=-\frac1{2p}.
$$

Thus the full [Fourier series](../../../../../../fourier-series-split.md) is

$$
\boxed{x\sin(px)=\frac{(-1)^{p+1}}p-\frac{\cos(px)}{2p}
+2p\!\sum_{\substack{n\geq1\\n\ne p}}
\frac{(-1)^{p+n}\cos(nx)}{n^2-p^2}}.
$$

This equality holds on $[-\pi,\pi]$ and by [periodicity](../../../../../../periodicity.md) everywhere. Indeed the [periodic extension](../../../../../../periodic-extension.md) is continuous at the joined endpoints, since both endpoint values are zero, and is piecewise smooth. The theorem on [pointwise convergence of a piecewise smooth Fourier series](../../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) therefore applies, including at the endpoints. The [Fourier coefficients](../../../../../../fourier-coefficient.md) also decay as $n^{-2}$, making the resulting [series](../../../../../../series-mathematics.md) absolutely and uniformly convergent.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
