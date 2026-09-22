<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every $\varphi\in\mathcal S$, the [change of variables formula](../../../../../../change-of-variables-formula.md) gives the identity

$$
\widehat{(A^t)^*\varphi}(x)
=\frac1{|\det A|}\widehat\varphi(A^{-1}x).
$$

Using this, the distributional Fourier transform, and the pullback formula from part b,

$$
\begin{aligned}
\langle\widehat{A^*u},\varphi\rangle
&=\frac1{|\det A|}
\langle u,(A^{-1})^*\widehat\varphi\rangle\\
&=\langle u,\widehat{(A^t)^*\varphi}\rangle
=\langle\widehat u,(A^t)^*\varphi\rangle\\
&=\left\langle
\frac{((A^t)^{-1})^*\widehat u}{|\det A|},
\varphi\right\rangle.
\end{aligned}
$$

Therefore

$$
\boxed{\widehat{A^*u}
=\frac{((A^t)^{-1})^*\widehat u}{|\det A|}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
