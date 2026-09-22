<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the [Fourier series](../../../../../../fourier-series-split.md)

$$
h(t)=\sum_{n\in\mathbb Z}\widehat h_n e^{i\pi nt}
$$

into the rectangle rule. The finite geometric sum obeys

$$
\frac1N\sum_{k=-N/2+1}^{N/2}
e^{2\pi ink/N}
=
\begin{cases}
1,&N\mid n,\\
0,&N\nmid n.
\end{cases}
$$

Consequently the quadrature value is

$$
\frac2N\sum_{k=-N/2+1}^{N/2}h(2k/N)
=2\sum_{j\in\mathbb Z}\widehat h_{jN},
$$

whereas

$$
\int_{-1}^1h(t)\,dt=2\widehat h_0.
$$

Thus the exact [Periodic N-point rectangle-rule error](../../../../../../periodic-n-point-rectangle-rule-error.md) is

$$
\boxed{
e_N(h)=-2\sum_{\substack{j\in\mathbb Z\\j\ne0}}
\widehat h_{jN}.}
$$

By the [Fourier coefficient decay of an analytic periodic function](../../../../../../fourier-coefficient-decay-of-an-analytic-periodic-function.md), there are constants $C>0$ and $0<\rho<1$ such that

$$
|\widehat h_n|\leq C\rho^{|n|}.
$$

It follows that

$$
|e_N(h)|
\leq4C\sum_{j=1}^{\infty}\rho^{jN}
=\frac{4C\rho^N}{1-\rho^N}.
$$

Therefore

$$
\boxed{|e_N(h)|=O(\rho^N),}
$$

which is exponential, and hence spectral, convergence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
