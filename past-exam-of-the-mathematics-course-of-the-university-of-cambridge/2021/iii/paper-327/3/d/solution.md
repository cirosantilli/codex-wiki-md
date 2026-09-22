<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md), write $A=O^tDO$ with $O$ [orthogonal](../../../../../../orthogonal-matrix.md) and $D=\operatorname{diag}(\xi_1,\ldots,\xi_n)$. Part a and the tensor-product property of the [Fourier transform](../../../../../../fourier-transform.md) give

$$
\mathcal F\left[e^{iDx\cdot x/2}\right](\lambda)
=\prod_{j=1}^n
\left(
\sqrt{\frac{2\pi}{|\xi_j|}}
e^{i\pi\operatorname{sgn}(\xi_j)/4}
e^{-i\lambda_j^2/(2\xi_j)}
\right).
$$

Thus

$$
\mathcal F\left[e^{iDx\cdot x/2}\right](\lambda)
=\sqrt{\frac{(2\pi)^n}{|\det D|}}
\exp\left[
\frac{i\pi}{4}\operatorname{sgn}(D)
-\frac i2D^{-1}\lambda\cdot\lambda
\right].
$$

Applying the pullback rule from part c to the orthogonal change of variables, for which $|\det O|=1$, replaces $D$ by $A$ and $D^{-1}$ by $A^{-1}$. Since determinant and [signature](../../../../../../signature-of-a-quadratic-form.md) are invariant under orthogonal conjugation,

$$
\boxed{
\left[e^{iAx\cdot x/2}\right]^{\widehat{}}(\lambda)
=\sqrt{\frac{(2\pi)^n}{|\det A|}}
\exp\left[
\frac{i\pi}{4}\operatorname{sgn}(A)
-\frac i2(A^{-1}\lambda)\cdot\lambda
\right]}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
