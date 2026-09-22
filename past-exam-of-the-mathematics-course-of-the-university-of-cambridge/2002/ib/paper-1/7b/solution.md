<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Fix real $y$ and use a rectangle with vertical sides at real coordinates $\pm R$. The function $e^{-z^2}$ is entire, so its closed [contour integral](../../../../../contour-integral.md) is zero by [Cauchy's integral theorem](../../../../../cauchy-s-integral-theorem.md). The bottom horizontal side contributes $\int_{-R}^Re^{-x^2}dx$ and the top contributes the negative of $\int_{-R}^Re^{-(x+iy)^2}dx$. This identity applies for either sign of $y$, with the corresponding oriented rectangle.

On a vertical side, $z=\pm R+is$ with $|s|\leq|y|$, and

$$
|e^{-z^2}|=e^{-R^2+s^2}\leq e^{-R^2+y^2}.
$$

The sum of the two vertical integrals in absolute value is at most $2|y|e^{-R^2+y^2}\to0$. Both horizontal improper integrals converge absolutely, since $|e^{-(x+iy)^2}|=e^{y^2}e^{-x^2}$. Letting $R\to\infty$ therefore proves

$$
\boxed{\int_{\mathbb R}e^{-(x+iy)^2}\,dx=\int_{\mathbb R}e^{-x^2}\,dx}.
$$

Complete the square in the [Fourier transform](../../../../../fourier-transform.md):

$$
\widehat f(y)=e^{-y^2/2}\int_{\mathbb R}e^{-(x+iy)^2/2}\,dx=e^{-y^2/2}\int_{\mathbb R}e^{-x^2/2}\,dx.
$$

The shifted-integral identity applies after scaling by $\sqrt2$. The [Gaussian integral](../../../../../gaussian-integral.md) is $\sqrt{2\pi}$: the square of $\int e^{-u^2}du$ becomes $2\pi\int_0^\infty e^{-r^2}r\,dr=\pi$ in polar coordinates. Thus the [Gaussian Fourier transform](../../../../../fourier-transform-of-a-gaussian.md) yields

$$
\boxed{\widehat f=\sqrt{2\pi}\,f}.
$$

The [eigenvalue](../../../../../eigenvalue.md) reflects the unnormalized transform convention in this question.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
