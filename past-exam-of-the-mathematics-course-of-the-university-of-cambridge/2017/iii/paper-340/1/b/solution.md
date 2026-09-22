<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $W_j=V_{j+1}\ominus V_j$ denote the [orthogonal complement](../../../../../../orthogonal-complement.md) of $V_j$ inside $V_{j+1}$. The [Meyer-Mallat theorem](../../../../../../meyer-mallat-theorem.md) constructs a [wavelet](../../../../../../wavelet.md) whose [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $W_0$. Dilation then gives the [orthogonal](../../../../../../orthogonal-vectors.md) decomposition into [orthogonal complements](../../../../../../orthogonal-complement.md) $L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j$, so its translates and dilates form an [orthonormal wavelet](../../../../../../orthonormal-wavelet.md) basis.

Using the [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md), choose the high-pass symbol $n(\xi)=e^{-i\xi}\overline{m(\xi+\pi)}$. The [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) identity makes the two analysis channels [orthonormal](../../../../../../orthonormal-set.md). The resulting [Fourier transform](../../../../../../fourier-transform.md) formula is

$$
\boxed{\widehat\psi(2\xi)=e^{-i\xi}\overline{m(\xi+\pi)}\widehat\varphi(\xi).}
$$

Equivalently, with the refinement coefficients from the [scaling refinement equation](../../../../../../scaling-refinement-equation.md), put $g_k=(-1)^{k-1}\overline{h_{1-k}}$ and $\psi(x)=\sqrt2\sum_kg_k\varphi(2x-k)$. This index choice gives precisely the displayed high-pass symbol. Changing all $g_k$ by one constant unit phase gives the same [orthonormal wavelet](../../../../../../orthonormal-wavelet.md) construction. In particular the often-used $(-1)^k\overline{h_{1-k}}$ convention differs only by a global minus sign. The basis is $\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k)$ for $j,k\in\mathbb Z$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
