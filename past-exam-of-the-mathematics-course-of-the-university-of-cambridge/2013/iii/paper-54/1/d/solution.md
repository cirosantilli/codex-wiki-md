<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\bar\nu=C r^a\Sigma^b$, the response is $q=b+1$. A nonaccreting background has $\bar\nu_0\Sigma_0\propto r^{-1/2}$, while $\Sigma_0\propto r^{-p}$, so

$$
\boxed{a-(b+1)p=-\tfrac12,\qquad a+\tfrac12=qp.}
$$

Consequently $\bar\nu_0\propto r^{p-1/2}$. On this steady background, introduce the [square-root-radius diffusion transform](../../../../../../square-root-radius-diffusion-transform.md)

$$
x=\sqrt r,\qquad g=\sqrt r\,\bar\nu_0\Sigma_1.
$$

Since $q$ is constant and $\partial_r=(2x)^{-1}\partial_x$, the [linear equation](../../../../../../linear-equation.md) becomes

$$
\partial_tg=3q\bar\nu_0 r^{-1/2}\partial_r(r^{1/2}\partial_rg)
=\frac{3q\bar\nu_0(r)}{4r}\partial_x^2g.
$$

Thus $A(x)\propto x^{2p-3}$, and the required choice is

$$
\boxed{p=\tfrac32,\qquad a=1+\tfrac32b,\qquad A=\frac{3q}{4}\frac{\bar\nu_0}r=\text{constant}.}
$$

For a [Fourier mode](../../../../../../fourier-mode.md) $g\propto e^{\lambda t+ik_xx}$, $\lambda=-Ak_x^2$. Positive [kinematic viscosity](../../../../../../kinematic-viscosity.md) makes $A$ have the sign of $q$, so $q<0$ gives growing modes whose rate increases with $k_x^2$. The formal equation is a [backward heat equation](../../../../../../backward-heat-equation.md) and predicts arbitrarily rapid small-scale amplification. Physically the [thin disc](../../../../../../thin-disk.md) diffusion closure applies only to [wavelengths](../../../../../../wavelength.md) sufficiently larger than the thickness and stress-relaxation scales; this formal limit identifies the need for a cutoff, rather than a finite fastest [wavelength](../../../../../../wavelength.md) absent from the model. The boundary case $q=0$ has vanishing linear transport response.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
