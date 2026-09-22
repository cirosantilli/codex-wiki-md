<h1 id="39a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Separate even and odd indices, using $\omega_{2m}^{2}=\omega_m$. Then

$$
\boxed{x_\ell=x_\ell^{(E)}+\omega_{2m}^{\ell}x_\ell^{(O)},\qquad
x_{\ell+m}=x_\ell^{(E)}-\omega_{2m}^{\ell}x_\ell^{(O)}}\quad(0\leq\ell<m).
$$

The second identity uses $\omega_{2m}^m=-1$. Each [FFT butterfly](../../../../../../fft-butterfly.md) uses one shared twiddle-factor product and two additions, so assembly costs $m$ multiplications and $2m$ additions.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [39A](../../39a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
