# Airy disk derivation

↑ **Parent:** [Airy disk](airy-disk.md)

Write $a=D/2$ and [wavenumber](wavenumber.md) $k=2\pi/\lambda$. The pupil [Fourier transform](fourier-transform-split.md), normalized by pupil [area](surface-area.md), gives the [Fraunhofer diffraction](fraunhofer-diffraction.md) [wave amplitude](wave-amplitude.md). In pupil [polar coordinates](polar-coordinates.md),

$$
A(u)=\frac1{\pi a^2}\int_0^a\int_0^{2\pi}e^{-ik\rho\sin\theta\cos\phi}\rho\,d\phi\,d\rho=2\int_0^1tJ_0(ut)\,dt,\qquad u=ka\sin\theta.
$$

The angular average is $J_0$ because $J_0(z)=(2\pi)^{-1}\int_0^{2\pi}e^{-iz\cos\phi}\,d\phi$. The [Bessel function of the first kind](bessel-function-of-the-first-kind.md) identity $d\{zJ_1(z)\}/dz=zJ_0(z)$ then reduces the radial [integral](integral-split.md) to $A(u)=2J_1(u)/u$. Taking the squared magnitude yields the [Airy disk](airy-disk.md) [light intensity](light-intensity.md) profile.[equations 10.78–10.84: angular integral, radial integral and Bessel identities](oscillations-and-waves-by-richard-fitzpatrick/two-dimensional-fourier-optics.md)

The apparent division by zero is removable. The [power series](power-series.md)

$$
J_1(u)=\frac u2-\frac{u^3}{16}+\frac{u^5}{384}+O(u^7)
$$

gives $A(u)=1-u^2/8+u^4/192+O(u^6)$ and $P(u)=1-u^2/4+5u^4/192+O(u^6)$. At the centre, every pupil contribution has the same [wave phase](phase-waves.md), so their normalized sum is one. The first dark ring instead corresponds to $J_1(u)=0$ with $u>0$, rather than to the removable zero of $J_1$ at the origin.

## ↑ Ancestors (7)

1. [Airy disk](airy-disk.md)
2. [Point spread function](point-spread-function-split.md)
3. [Physical optics](physical-optics-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Airy disk](airy-disk.md)
- [Incoherent two-source Airy profile](incoherent-two-source-airy-profile.md)
