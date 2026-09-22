<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a literal domain error in the printed formula. A [semivariogram](../../../../../../semivariogram.md) indexed by a signed displacement must satisfy $\gamma(h)=\gamma(-h)$, since reversing the two observations leaves the squared increment unchanged. For positive $\sigma^2$ or $\tau^2$, the displayed positive-lag value is nonzero whereas the displayed negative-lag value is zero. Thus the claim on all of $\mathbb R$ is false as written.

Interpret the argument as a nonnegative distance, or use the even extension of the [Gaussian semivariogram](../../../../../../gaussian-semivariogram.md). For $\sigma^2,\tau^2\ge0$ and $\phi>0$, the intended model is

$$
\gamma(h)=\tau^2\mathbf1_{\{h\ne0\}}+\sigma^2(1-e^{-\phi^2h^2}).
$$

It admits the [covariogram](../../../../../../covariogram.md)

$$
\boxed{C(h)=\sigma^2e^{-\phi^2h^2}+\tau^2\mathbf1_{\{h=0\}}.}
$$

The [Gaussian kernel](../../../../../../gaussian-kernel.md) is a [positive-definite kernel](../../../../../../positive-semidefinite-kernel.md), as can be seen from the [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md): in one dimension

$$
e^{-\phi^2h^2}=\int_{\mathbb R}e^{i\omega h}\frac{e^{-\omega^2/(4\phi^2)}}{2\phi\sqrt\pi}\,d\omega,
$$

and the nonnegative spectral density makes every finite [covariance](../../../../../../covariance.md) quadratic form nonnegative. In higher dimensions use the product Gaussian density. Adding independent Gaussian [white noise](../../../../../../white-noise.md) of [variance](../../../../../../variance-split.md) $\tau^2$ adds the diagonal nugget [covariance](../../../../../../covariance.md). Thus a zero-mean [stationary Gaussian random field](../../../../../../stationary-gaussian-random-field.md) exists with this [covariance](../../../../../../covariance.md), and $C(0)-C(h)$ gives the corrected [semivariogram](../../../../../../semivariogram.md).

For nonzero structured [variance](../../../../../../variance-split.md), the [nugget effect](../../../../../../nugget-effect.md) is the right limit $\tau^2$ at zero, the [sill of a semivariogram](../../../../../../sill-of-a-semivariogram.md) is $\tau^2+\sigma^2$, and the [range of a semivariogram](../../../../../../range-of-a-semivariogram.md) is infinite if defined as the distance at which the sill is exactly reached. A 95-percent [practical range](../../../../../../practical-range.md) solves $1-e^{-\phi^2h^2}=0.95$:

$$
\boxed{h_{0.95}=\sqrt{\log20}/\phi.}
$$

The scale $1/\phi$ is sometimes called the range parameter; it is neither the exact range nor the 95-percent practical range. If $\sigma^2=0$, there is no nontrivial structured range.

The fact that [a semivariogram does not determine stationarity](../../../../../../a-semivariogram-does-not-determine-stationarity.md) is a further distinction: a [semivariogram](../../../../../../semivariogram.md) specifies increment variation, not a unique process or absolute [covariance](../../../../../../covariance.md). Adding an independent random constant adds a constant to $C$ without changing $\gamma$. More strongly, subtracting $W(0)$ from a stationary field $W(s)$ preserves its [semivariogram](../../../../../../semivariogram.md) but generally makes its [variance](../../../../../../variance-split.md) depend on $s$. The corrected statement is that this [semivariogram](../../../../../../semivariogram.md) admits a second-order stationary model, with the displayed [covariance](../../../../../../covariance.md) using the usual convention $C(h)\to0$ at large distance; it does not force every compatible process to be stationary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
