<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed mode numbers $k,l$, expansion of the [sines](../../../../../../sine.md) gives

$$
\lambda_{5,kl}=-\pi^2(k^2+l^2)+\frac{\pi^4h^2}{12}(k^4+l^4)+O(h^4),
$$

whereas the mixed [Kronecker product](../../../../../../kronecker-product.md) correction gives

$$
\lambda_{9,kl}=-\pi^2(k^2+l^2)+\frac{\pi^4h^2}{12}(k^2+l^2)^2+O(h^4).
$$

Thus **both [eigenvalue](../../../../../../eigenvalue.md) approximations are second order for fixed modes**. The leading nine-point error includes an additional positive term $\pi^4h^2k^2l^2/6$.

There is also an exact comparison, not just an asymptotic one. Since $\sin x<x$ for $0<x<\pi/2$, and both sine factors in the correction are positive,

$$
-\pi^2(k^2+l^2)<\lambda_{5,kl}<\lambda_{9,kl}.
$$

Both estimates lie on the less-negative side of the continuum [Laplacian](../../../../../../laplacian.md) [eigenvalue](../../../../../../eigenvalue.md), so **the five-point formula is the better [eigenvalue](../../../../../../eigenvalue.md) estimate for every corresponding interior mode**. The [five-point versus nine-point Laplacian eigenvalue accuracy](../../../../../../five-point-versus-nine-point-laplacian-eigenvalue-accuracy.md) comparison does not contradict the useful isotropy or special Poisson accuracy properties of a nine-point stencil. Those properties concern a different error criterion. The fixed-mode expansion is not uniform for modes with $k$ or $l$ comparable to $h^{-1}$; wavelengths close to the mesh scale need not have small relative spectral error.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
