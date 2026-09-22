<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $v=0$ and use amplitudes proportional to $e^{i(kx+mz-\omega t)}$. Zonal momentum gives

$$
\hat u=\frac{k}{\omega}\hat\phi,
$$

while incompressibility, buoyancy evolution, and hydrostatic balance give

$$
\hat w=-\frac{k}{m}\hat u
=-\frac{\omega m}{N^2}\hat\phi.
$$

Hence

$$
\omega^2=\frac{N^2k^2}{m^2}.
$$

Meridional geostrophic balance requires

$$
\frac{d\hat\phi}{dy}
=-\frac{\beta k}{\omega}y\hat\phi,
$$

so

$$
\boxed{
\hat\phi(y)=\Phi_0
\exp\left(-\frac{\beta k}{2\omega}y^2\right)}.
$$

Decay as $|y|\to\infty$, together with $\beta>0$ and $k>0$, requires $\omega>0$. Therefore

$$
\boxed{\omega=\frac{Nk}{|m|}},
\qquad
\boxed{
\hat\phi(y)=\Phi_0
\exp\left(-\frac{\beta|m|}{2N}y^2\right)}.
$$

The negative-frequency root makes the Gaussian exponent positive and the solution diverge away from the equator. The acceptable branch is the eastward [equatorial Kelvin wave](../../../../../../equatorial-kelvin-wave.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
