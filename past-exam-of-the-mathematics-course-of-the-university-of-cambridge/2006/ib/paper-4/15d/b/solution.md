<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrating the interval indicator gives

$$
\boxed{\hat f_1(\lambda)=\frac{2\sin(\lambda/2)}{\lambda},\quad\hat f_1(0)=1.}
$$

The [convolution](../../../../../../convolution.md) $f_2(x)$ is the length of overlap of two intervals of length one whose centres differ by $x$. Thus $f_2(x)=1-|x|$ for $|x|\leq1$, and zero otherwise. The [convolution theorem](../../../../../../convolution-theorem.md) gives

$$
\boxed{\hat f_2(\lambda)=\left(\frac{2\sin(\lambda/2)}{\lambda}\right)^2.}
$$

For this [Fourier transform](../../../../../../fourier-transform.md) normalization, the [Parseval identity](../../../../../../parseval-identity.md) says $\int|f|^2dx=(2\pi)^{-1}\int|\hat f|^2d\lambda$. Since

$$
\int|f_2(x)|^2dx=2\int_0^1(1-x)^2dx=\frac23,
$$

we have $\int|\hat f_2|^2d\lambda=4\pi/3$. Substituting $\lambda=2y$ gives

$$
2\int_{-\infty}^{\infty}\left(\frac{\sin y}{y}\right)^4dy=\frac{4\pi}{3},
\qquad\boxed{\int_{-\infty}^{\infty}\left(\frac{\sin y}{y}\right)^4dy=\frac{2\pi}{3}.}
$$

The quotient at zero is understood by its continuous limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
