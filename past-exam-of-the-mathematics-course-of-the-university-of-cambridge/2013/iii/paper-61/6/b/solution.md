<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original PDF has indices $3^k$; the exponent is lost in the TeX transcription. This lacunary indexing is essential to the [positive lacunary Chebyshev series](../../../../../../positive-lacunary-chebyshev-series.md) argument below.

Let $K$ be the least nonnegative integer with $3^K>n$, so $K=0$ for $n=0$. Define

$$
p_n(x)=\sum_{k=0}^{K-1}a_kT_{3^k}(x),\qquad
A_K=\sum_{k=K}^{\infty}a_k.
$$

For $K=0$ the sum is empty and means the zero [polynomial](../../../../../../polynomial-split.md). Each included [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) has degree at most $n$. Also $|T_j(x)|\le1$ on the interval, so summability of the positive coefficients gives [uniform convergence](../../../../../../uniform-convergence.md) by the [Weierstrass M-test](../../../../../../weierstrass-m-test.md), and

$$
\|f_0-p_n\|_\infty\le A_K.
$$

Choose $L=3^K$ and the $L+1$ points $x_j=\cos(j\pi/L)$, $0\le j\le L$. For every omitted index $k\ge K$, the integer $3^{k-K}$ is odd. Consequently,

$$
T_{3^k}(x_j)=\cos(3^{k-K}j\pi)=(-1)^j.
$$

Every term of the tail has the same sign at a given point, and therefore

$$
f_0(x_j)-p_n(x_j)=(-1)^jA_K.
$$

This shows both that the error norm is exactly $A_K$ and that it alternates at $L+1\ge n+2$ distinct points. The points are in decreasing order; reversing their order still gives alternation. The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) proves that this partial sum is the unique [best uniform approximation](../../../../../../best-uniform-approximation.md). Hence

$$
\boxed{p_n=\sum_{3^k\le n}a_kT_{3^k},\qquad
E_n(f_0)=\sum_{3^k>n}a_k}.
$$

In particular, $p_0=0$ and $E_0(f_0)=\sum_{k=0}^\infty a_k$. The equal signs of all tail terms at the same extrema are the reason positivity and the odd integer frequency ratios are useful.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
