<h1 id="20f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $n\geq1$, the [convolution](../../../../../../convolution.md) equals the length of the overlap of two intervals:

$$
 g_n(\xi)=\begin{cases}2,&|\xi|\leq n-1,\\n+1-|\xi|,&n-1<|\xi|<n+1,\\0,&|\xi|\geq n+1.\end{cases}
$$

It is [continuous](../../../../../../continuous-function.md) and compactly supported, with $\|g_n\|_\infty=2$. Inverse [Fourier transform](../../../../../../fourier-transform.md) turns this [convolution](../../../../../../convolution.md) into a product, so

$$
\boxed{h_n(x)=\frac{\sin(2\pi n x)\sin(2\pi x)}{\pi^2x^2}\ (x\ne0),\qquad h_n(0)=4n.}
$$

This function is bounded near zero and $O(x^{-2})$ at infinity, hence lies in $L^1$. [Fourier inversion](../../../../../../fourier-inversion-theorem.md), or the [convolution theorem](../../../../../../convolution-theorem.md) applied first to the integrable interval indicators, gives $\widehat h_n=g_n$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
