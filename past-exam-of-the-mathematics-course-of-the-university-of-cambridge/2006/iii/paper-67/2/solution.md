<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a continuous $2\pi$-periodic [function](../../../../../function-split.md), define the [Fourier coefficients](../../../../../fourier-coefficient.md) and [Fourier partial sum](../../../../../fourier-partial-sum.md) by

$$
\widehat f(k)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-ikt}\,dt,\qquad
s_n(f;x)=\sum_{|k|\leq n}\widehat f(k)e^{ikx}.
$$

The [Fejér sum](../../../../../fejer-sum.md) is the arithmetic average of the first $n$ [Fourier partial sums](../../../../../fourier-partial-sum.md):

$$
\boxed{\sigma_n(f)=\frac1n\sum_{j=0}^{n-1}s_j(f)
=\sum_{|k|<n}\left(1-\frac{|k|}{n}\right)\widehat f(k)e^{ikx}.}
$$

Thus $s_n$ has degree at most $n$, whereas $\sigma_n$ has degree at most $n-1$. These indexing conventions matter in the identity in (b). Throughout, $m$ is a positive integer; when $n=0$, any term $n\sigma_n$ is interpreted as zero without introducing $\sigma_0$.

For later estimates, the [Fejér kernel](../../../../../fejer-kernel.md) in the PDF's normalization is

$$
F_n(t)=\frac1{2n}\left|\sum_{j=0}^{n-1}e^{ijt}\right|^2
=\frac1{2n}\frac{\sin^2(nt/2)}{\sin^2(t/2)},\qquad
\sigma_n(f;x)=\frac1\pi\int_{-\pi}^{\pi}f(x-t)F_n(t)\,dt.
$$

The apparent singularities are removable. The squared modulus makes $F_n$ nonnegative, and integrating its finite exponential expansion leaves only the $n$ diagonal terms, so $\pi^{-1}\int F_n=1$. In particular [Fejér summation is a uniform-norm contraction](../../../../../fejer-summation-is-a-uniform-norm-contraction.md):

$$
\|\sigma_nf\|_\infty\leq\frac1\pi\int_{-\pi}^{\pi}F_n(t)\|f\|_\infty\,dt=\|f\|_\infty.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
