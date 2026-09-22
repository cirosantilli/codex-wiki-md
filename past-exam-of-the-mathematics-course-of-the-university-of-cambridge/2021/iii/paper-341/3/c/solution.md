<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Split the generator as $iA-iV$. One [Strang splitting](../../../../../../strang-splitting.md) step is

$$
\boxed{
\mathbf u^{n+1}
=e^{-ihV/2}e^{ihA}e^{-ihV/2}\mathbf u^n
}.
$$

The two potential half-steps are componentwise multiplications. The circulant matrix $A$ is diagonalized by the [discrete Fourier transform](../../../../../../discrete-fourier-transform.md); its eigenvalues are

$$
\lambda_j=-4M^2\sin^2\left(\frac{\pi j}{2M}\right),
\qquad j=0,\ldots,2M-1.
$$

Thus the middle step consists of a [Fast Fourier transform](../../../../../../cooley-tukey-fft-algorithm.md), multiplication of Fourier coefficient $j$ by $e^{ih\lambda_j}$, and an inverse transform. Its cost is $O(M\log M)$ and every factor is unitary, so the implementation preserves the discrete norm exactly up to roundoff.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
