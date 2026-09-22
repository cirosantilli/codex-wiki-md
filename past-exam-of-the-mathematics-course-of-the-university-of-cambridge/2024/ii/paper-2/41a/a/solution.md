<h1 id="41a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The exact average is $I(h)=\widehat h_0$. For one Fourier mode,

$$
\frac1{2N}\sum_{k=-N+1}^Ne^{i\pi nk/N}
=\begin{cases}
1,&2N\mid n,\\
0,&2N\nmid n.
\end{cases}
$$

Thus the [periodic trapezoidal Fourier aliasing](../../../../../../periodic-trapezoidal-fourier-aliasing.md) identity gives

$$
I_N(h)=\sum_{j\in\mathbb Z}\widehat h_{2Nj},
\qquad
\boxed{|I_N(h)-I(h)|
=\left|\sum_{j\ne0}\widehat h_{2Nj}\right|}.
$$

Under the coefficient bound,

$$
|I_N-I|
\leq2M\sum_{j=1}^\infty c^{2Nj}
=\boxed{\frac{2Mc^{2N}}{1-c^{2N}}}
\leq\frac{2M}{1-c^2}c^{2N}.
$$

This decays exponentially in $N$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41A](../../41a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
