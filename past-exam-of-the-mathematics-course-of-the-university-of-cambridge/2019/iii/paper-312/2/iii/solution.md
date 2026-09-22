<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the imaginary-axis contour of the inverse transform of the [moment-generating function](../../../../../../moment-generating-function.md), $J=iy$, so the Gaussian part gives the [normal distribution](../../../../../../normal-distribution.md)

$$
p_G(\delta)=\frac1{\sqrt{2\pi}\sigma}
\exp\left(-\frac{\delta^2}{2\sigma^2}\right).
$$

Because $J^3e^{-J\delta}=-\partial_\delta^3e^{-J\delta}$, the first non-Gaussian term is

$$
\boxed{p(\delta)=\left(1-\frac{S_3\sigma^4}{6}\partial_\delta^3\right)p_G(\delta)}.
$$

Differentiating the Gaussian three times gives

$$
p_G'''(\delta)=
\left(-\frac{\delta^3}{\sigma^6}+\frac{3\delta}{\sigma^4}\right)p_G(\delta).
$$

Hence the [Edgeworth expansion](../../../../../../edgeworth-series.md) is

$$
\boxed{
p(\delta)=\frac{e^{-\delta^2/(2\sigma^2)}}{\sqrt{2\pi}\sigma}
\left[1+\frac{S_3}{6\sigma^2}
(\delta^3-3\delta\sigma^2)\right]}.
$$

Equivalently its correction is $(S_3\sigma/6)\operatorname{He}_3(\delta/\sigma)$, with $\operatorname{He}_3(z)=z^3-3z$, a [Probabilists' Hermite polynomial](../../../../../../probabilists-hermite-polynomial.md). It integrates to zero and reproduces the third [moment](../../../../../../moment.md) $S_3\sigma^4$. The expansion is intended for weak non-Gaussianity in the bulk, rather than the far tails.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
