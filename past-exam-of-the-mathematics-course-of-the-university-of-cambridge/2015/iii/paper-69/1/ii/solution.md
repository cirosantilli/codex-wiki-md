<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Averaging the given [Dirichlet kernels](../../../../../../dirichlet-kernel.md) gives the normalized [Fejér kernel](../../../../../../fejer-kernel.md)

$$
K_n(t)=\frac1{\pi n}\sum_{j=0}^{n-1}D_j(t)
=\frac1{2\pi n}\left(\frac{\sin(nt/2)}{\sin(t/2)}\right)^2.
$$

The geometric-series identity, or summing the sine terms, proves the second equality. At multiples of $2\pi$ use its removable value $n/(2\pi)$. Therefore $K_n\geq0$, and

$$
\sigma_n(f,x)=\int_{-\pi}^{\pi}K_n(t)f(x-t)\,dt
$$

is a [positive linear operator on continuous functions](../../../../../../positive-linear-operator-on-continuous-functions.md). The [Fourier partial sums](../../../../../../fourier-partial-sum.md), viewed as [orthogonal projections](../../../../../../orthogonal-projection.md), fix $1$, so $\sigma_n1=1$ and $\int K_n=1$. They also fix $\sin x$ and $\cos x$ for degrees at least one, whereas $s_0$ annihilates them. Consequently

$$
\sigma_n(\sin x)=(1-1/n)\sin x,\qquad
\sigma_n(\cos x)=(1-1/n)\cos x.
$$

All three periodic [Korovkin theorem](../../../../../../korovkin-theorem.md) tests converge uniformly. Hence **[Fejér sums](../../../../../../fejer-sum.md) converge uniformly for every continuous periodic function**:

$$
\boxed{\|\sigma_n(f)-f\|_\infty\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
