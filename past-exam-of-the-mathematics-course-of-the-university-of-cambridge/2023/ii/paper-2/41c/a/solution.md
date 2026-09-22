<h1 id="41c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the two-periodic [Fourier series](../../../../../../fourier-series-split.md), orthogonality of the exponential basis gives the [Fourier coefficient](../../../../../../fourier-coefficient.md)

$$
\boxed{\widehat c_n=\frac12\int_{-1}^{1}c(x)e^{-i\pi nx}\,dx},
$$

where any interval of length two could replace $[-1,1]$.

Let $C_{nm}=\widehat c_{n-m}$ for $-d\leq n,m\leq d$. Since $c$ is real,

$$
\widehat c_{-k}=\overline{\widehat c_k},
$$

so $C_{mn}=\overline{C_{nm}}$ and $C$ is a [Hermitian matrix](../../../../../../hermitian-positive-definite-matrix.md). For any nonzero $z=(z_{-d},\ldots,z_d)^T$,

$$
\begin{aligned}
z^*Cz
&=\sum_{n,m=-d}^d\overline{z_n}\widehat c_{n-m}z_m\\
&=\frac12\int_{-1}^{1}c(x)
\left|\sum_{m=-d}^dz_me^{i\pi mx}\right|^2dx.
\end{aligned}
$$

The [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) in the modulus cannot vanish identically unless every $z_m$ vanishes. Since $c(x)>0$, the integral is strictly positive. Hence $C$ is [Hermitian positive definite](../../../../../../hermitian-positive-definite-matrix.md), which is the [positive Fourier-symbol Toeplitz matrix](../../../../../../positive-fourier-symbol-toeplitz-matrix.md) result.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41C](../../41c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
