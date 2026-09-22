<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Let $\omega=e^{2\pi i/N}$. Using the convention

$$
\widehat x_k=\sum_{n=0}^{N-1}x_n\omega^{-kn},
\qquad 0\leq k<N,
$$

the [discrete Fourier transform](../../../../../discrete-fourier-transform.md) of the supplied sequence follows from the [binomial theorem](../../../../../binomial-theorem.md):

$$
x_n=\frac1N\sum_{m=0}^{N-1}\binom{N-1}{m}\omega^{mn}.
$$

The [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md) gives

$$
\sum_{n=0}^{N-1}\omega^{(m-k)n}
=\begin{cases}N,&m=k,\\0,&m\ne k.\end{cases}
$$

Since $m,k$ both lie between zero and $N-1$, it follows that

$$
\boxed{\widehat x_k=\binom{N-1}{k}},
\qquad k=0,\ldots,N-1.
$$

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
