<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same negative-exponent [Fourier transform](../../../../../../fourier-transform.md) as in the preceding part and let $f=d\log D_+/d\log a$. In linear theory, $\dot\delta=Hf\delta$, and the [linearized cosmological continuity equation](../../../../../../linearized-cosmological-continuity-equation.md) is $\dot\delta+a^{-1}\nabla_x\cdot\mathbf v=0$. Its irrotational solution is

$$
\mathbf v_{\mathbf k}=-iaHf\frac{\mathbf k}{k^2}\delta_{\mathbf k},
\qquad
\mathbf v(\mathbf r)=aHf\nabla_r\int\frac{d^3k}{(2\pi)^3}\frac{\delta_{\mathbf k}}{k^2}e^{-i\mathbf k\cdot\mathbf r}.
$$

Here $\mathbf r$ labels the comoving spatial position for the Fourier expansion. The quantity being differentiated is also $-\Phi/(4\pi Ga^2\bar\rho)$, by the [Poisson equation](../../../../../../poisson-equation.md); thus this explicitly obtains the velocity from the Fourier components of the [peculiar gravitational potential](../../../../../../peculiar-gravitational-potential.md).

Conjugating the [Rayleigh plane-wave expansion](../../../../../../rayleigh-plane-wave-expansion.md), and using the symmetric addition formula for [spherical harmonics](../../../../../../spherical-harmonic.md), gives

$$
e^{-i\mathbf k\cdot\mathbf r}=4\pi\sum_{\ell m}(-i)^\ell j_\ell(kr)Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).
$$

For the radial component $U=\mathbf v\cdot\hat r$, differentiate at fixed angular position. Only the [Spherical Bessel function](../../../../../../spherical-bessel-function.md) depends on $r$, and $d j_\ell(kr)/dr=k j_\ell'(kr)$. Therefore the [radial peculiar velocity in spherical harmonics](../../../../../../radial-peculiar-velocity-in-spherical-harmonics.md) is

$$
\boxed{U(\mathbf r)=\frac{aHf}{2\pi^2}\sum_{\ell m}(-i)^\ell
\int d^3k\,\frac{\delta_{\mathbf k}}{k}\frac{d j_\ell(kr)}{d(kr)}
Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).}
$$

The coefficient is $4\pi/(2\pi)^3=1/(2\pi^2)$, and $(-i)^\ell=(i^\ell)^*$, so the phase and conjugation agree with the requested expression. At the present epoch, $a=1$ and $H=H_0$. Adopting the traditional approximation $f\simeq\Omega_m^{0.6}$ gives

$$
\frac{U}{H_0}\simeq\frac{\Omega_m^{0.6}}{2\pi^2}\sum_{\ell m}(i^\ell)^*
\int d^3k\,\frac{\delta_{\mathbf k}}{k}j_\ell'(kr)
Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).
$$

The printed expression is therefore the present-epoch result in units with $H_0=1$, or with its velocity interpreted as $U/H_0$. For distances and velocities in ordinary physical units, it needs the factor $H_0$; at a general epoch it needs $aH$. The approximation $f\simeq\Omega_m^{0.6}$ is exact in the Einstein-de Sitter limit but is not an exact growth formula for arbitrary cosmologies.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
