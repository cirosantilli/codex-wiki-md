<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $z=x_0+iy$. Since $|M(z)|\leq\mathbb Ee^{x_0\xi}$ and $|z(z-1)|^{-1}$ is integrable over $y\in\mathbb R$, the proposed contour integral is absolutely convergent. The same bound justifies the [Fubini's theorem](../../../../../../fubini-s-theorem.md) when substituting $M(z)=\mathbb Ee^{z\xi}$:

$$
\begin{aligned}
\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{M(z)}{z(z-1)e^{(z-1)k}}\,dz
&=e^k\mathbb E\!\left[\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{e^{z(\xi-k)}}{z(z-1)}\,dz\right]\\
&=e^k\mathbb E(e^{\xi-k}-1)^+=C(k).
\end{aligned}
$$

The last equality uses the contour identity provided in the original PDF. Consequently

$$
\boxed{C(k)=\frac1{2\pi i}\int_{x_0-i\infty}^{x_0+i\infty}\frac{M(z)}{f(z,k)}\,dz\qquad(x_0>1).}
$$

This is [contour inversion for call prices](../../../../../../contour-inversion-for-call-prices.md). The supplied TeX corrupts the permitted identity into a reciprocal and drops the imaginary units from its endpoints; the PDF has $(e^a-1)^+$ and the vertical contour used above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
