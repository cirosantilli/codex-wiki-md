# Airy disk normalization and encircled energy

↑ **Parent:** [Airy disk](airy-disk.md)

Peak normalization $P(0)=1$ does not make the [integral](integral-split.md) of a [point spread function](point-spread-function-split.md) equal to one. In the [paraxial approximation](paraxial-approximation.md) to the [focal plane](focal-plane.md), define $b=\pi D/(\lambda f)$ and $u=br$. The unit-[integral](integral-split.md) [point spread function normalization](point-spread-function-normalization.md) is

$$
p(r)=\frac{b^2}{4\pi}P(br),\qquad \int_{\mathbb R^2}p(r)\,d^2\mathbf r=1.
$$

Here $p$ has units of inverse [area](surface-area.md); multiplying by the detected [radiant flux](radiant-flux.md) gives image-plane [irradiance](irradiance.md). Its [encircled energy](encircled-energy.md), meaning the fraction inside radius $R=U/b$, is

$$
E(U)=\int_0^{U/b}2\pi r p(r)\,dr=\frac12\int_0^UuP(u)\,du=1-J_0(U)^2-J_1(U)^2.
$$

This is an [integral](integral-split.md) over [area](surface-area.md), so its radial weight is $u$. An unweighted [integral](integral-split.md) of a line through the centre is a different quantity.

A short proof uses the [Bessel function of the first kind](bessel-function-of-the-first-kind.md) identities $J_0'=-J_1$ and $J_1'=J_0-J_1/u$. They give

$$
\frac{d}{dU}\left(1-J_0(U)^2-J_1(U)^2\right)=\frac{2J_1(U)^2}{U}=\frac U2P(U).
$$

Both expressions for $E$ vanish at zero. Since these [Bessel functions of the first kind](bessel-function-of-the-first-kind.md) tend to zero as $U\to\infty$, $E(\infty)=1$, establishing the normalization. At the first dark ring,

$$
E(j_{1,1})=1-J_0(j_{1,1})^2\simeq0.837784869.
$$

A circular detector region ending at the first zero therefore misses about $16.22\%$ of the ideal [radiant flux](radiant-flux.md), even though the surrounding rings have low peak [light intensity](light-intensity.md). This matters when converting measured counts into total source brightness or choosing an image aperture for a [photodetector](photodetector.md).

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
