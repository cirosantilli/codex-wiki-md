<h1 id="6/b/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $F(t)=\sum_{k\in\mathbb Z}|f(t+2\pi k)|^2$. By the [Tonelli theorem](../../../../../../../tonelli-theorem.md), $F$ is integrable on $[0,2\pi]$, since its integral is $\int_{\mathbb R}|f|^2<\infty$. The [Plancherel theorem](../../../../../../../plancherel-theorem.md) and periodization give

$$
\langle\phi(\cdot-n),\phi(\cdot-m)\rangle
=\frac1{2\pi}\int_{\mathbb R}|f(t)|^2e^{i(m-n)t}\,dt
=\frac1{2\pi}\int_0^{2\pi}F(t)e^{i(m-n)t}\,dt.
$$

Consequently, if $F=1$ almost everywhere these [inner products](../../../../../../../inner-product.md) are $\delta_{mn}$, proving [orthonormality](../../../../../../../orthonormal-set.md). Conversely [orthonormality](../../../../../../../orthonormal-set.md) says that every [Fourier coefficient](../../../../../../../fourier-coefficient.md) of $F-1$ is zero. The [uniqueness of Fourier coefficients in L1](../../../../../../../uniqueness-of-fourier-coefficients-in-l1.md) implies $F-1=0$ almost everywhere. Hence

$$
\boxed{\{\phi(\cdot-n)\}_{n\in\mathbb Z}\text{ is orthonormal}\quad\Longleftrightarrow\quad\sum_k|f(t+2\pi k)|^2=1\text{ a.e.}}
$$

This proves [orthonormal translates and Fourier periodization](../../../../../../../orthonormal-translates-and-fourier-periodization.md), including both directions and the normalization constant associated with the printed [Fourier transform](../../../../../../../fourier-transform.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 70](../../../../paper-70-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
