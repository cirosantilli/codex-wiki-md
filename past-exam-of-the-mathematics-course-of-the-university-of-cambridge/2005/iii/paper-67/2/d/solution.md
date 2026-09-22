<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two boundary values have jump

$$
J(\theta)=\mu(\lambda^+)-\mu(\lambda^-)=-iHRf(\rho,\theta).
$$

The line-tail contributions cancel. Because the [complexified transport Cauchy kernel](../../../../../../complexified-transport-cauchy-kernel.md) is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on both sides of the unit circle and vanishes at spectral infinity, the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) reconstructs it from this jump:

$$
\mu(\lambda)=\frac1{2\pi i}\oint_{|\zeta|=1}\frac{J(\arg\zeta)}{\zeta-\lambda}d\zeta.
$$

There is no additional entire term: its inside and outside boundary values would agree, so it would define an entire function vanishing at infinity. Expand outside the circle as $\mu=\mu_1/\lambda+O(\lambda^{-2})$. Then

$$
\mu_1=-\frac1{2\pi}\int_0^{2\pi}e^{i\theta}J(\theta)d\theta
=\frac{i}{2\pi}\int_0^{2\pi}e^{i\theta}HRf(\rho,\theta)d\theta.
$$

In the original coordinate $w=x_1+ix_2$, the [transport equation](../../../../../../transport-equation.md) is $(\lambda\partial_w+\lambda^{-1}\partial_{\bar w})\mu=f$. Its constant term at infinity is $\partial_w\mu_1=f$. Since

$$
\partial_w\rho=\frac12(\partial_{x_1}-i\partial_{x_2})\rho=-\frac i2e^{-i\theta},
$$

we obtain the **inverse Radon transform** in [filtered backprojection](../../../../../../filtered-backprojection.md) form:

$$
\boxed{f(x_1,x_2)=\frac1{4\pi}\int_0^{2\pi}
(\partial_\rho HRf)(-x_1\sin\theta+x_2\cos\theta,\theta)d\theta.}
$$

Opposite directions represent the same unoriented line. Reversing $\theta$ by $\pi$ reverses $\rho$; the [Hilbert transform](../../../../../../hilbert-transform.md) changes sign under this reversal, and its derivative changes it back. Thus the integrand agrees for opposite directions and the factor becomes $1/(2\pi)$ if the angular integral is over $[0,\pi)$. With the convention $\widehat h(\kappa)=\int e^{-i\kappa\rho}h(\rho)d\rho$, the [Hilbert transform](../../../../../../hilbert-transform.md) has [Fourier multiplier](../../../../../../fourier-multiplier.md) $-i\operatorname{sgn}\kappa$; the derivative makes the filter $|\kappa|$. This also identifies the formula with the standard ramp-filter reconstruction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
