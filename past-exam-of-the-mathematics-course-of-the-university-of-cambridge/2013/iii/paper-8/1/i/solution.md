<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use normalized [Fourier coefficients](../../../../../../fourier-coefficient.md) and the [inner product](../../../../../../inner-product.md)

$$
\widehat f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-int}\,dt,\qquad
\langle f,g\rangle=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)\overline{g(t)}\,dt.
$$

The functions $e_n(t)=e^{int}$ are [orthonormal](../../../../../../orthonormal-set.md). Hence the [Fourier partial sum](../../../../../../fourier-partial-sum.md) $S_Nf=\sum_{|n|\leq N}\widehat f(n)e_n$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the [trigonometric polynomials](../../../../../../trigonometric-polynomial.md) of degree at most $N$. For any such polynomial $P$, [orthogonality](../../../../../../orthogonal-vectors.md) gives

$$
\|f-P\|_2^2=\|f-S_Nf\|_2^2+\|S_Nf-P\|_2^2,
$$

so $\|f-S_Nf\|_2\leq\|f-P\|_2$.

Given $\varepsilon>0$, the permitted density result supplies a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $P$ with $\|f-P\|_\infty<\varepsilon$. Once $N$ includes its degree,

$$
\|f-S_Nf\|_2\leq\|f-P\|_2\leq\|f-P\|_\infty<\varepsilon.
$$

Therefore **the [Fourier partial sums](../../../../../../fourier-partial-sum.md) converge to $f$ in the normalized $L^2$ norm**, giving exactly the stated mean-square limit.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
