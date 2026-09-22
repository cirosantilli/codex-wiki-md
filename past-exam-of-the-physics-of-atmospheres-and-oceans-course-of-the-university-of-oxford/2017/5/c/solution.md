<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work with the explicitly corrected reduced-pressure system in [b](../b.md). Write $d=1/(2H)$ and use the complex wave amplitude, taking real parts at the end. The vertical factor satisfies $(\partial_z^2-H^{-1}\partial_z)w=-(m^2+d^2)w$, so the wave equation gives

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2+d^2},\qquad
c=\frac\omega k=\frac{N}{\sqrt{k^2+m^2+d^2}}>0.}
$$

For a [Kelvin wave](../../../../equatorial-kelvin-wave.md), continuity, zonal momentum and the [buoyancy](../../../../buoyancy.md) equation then determine all polarizations:

$$
\boxed{u=-\frac{m+id}{k}\,w,\qquad
\Phi=\frac\omega k u=-\frac{\omega(m+id)}{k^2}w,
\qquad p'=\rho_0\Phi,\qquad b=-i\frac{N^2}{\omega}w,\qquad v=0.}
$$

In particular $u,w,b,\Phi$ have amplitude proportional to $e^{z/(2H)}$, whereas [pressure](../../../../pressure-split.md) $p'$ has amplitude proportional to $e^{-z/(2H)}$. Directly substituting these expressions into vertical momentum gives $\Phi_z=-i\omega(m^2+d^2)w/k^2=i(\omega-N^2/\omega)w$, verifying both the sign and the [dispersion relation](../../../../dispersion-relation-split.md).

Meridional momentum is $\beta yu+\Phi_y=0$. Since $\Phi=cu$, it integrates to a [Gaussian](../../../../normal-distribution.md) $\exp[-\beta y^2/(2c)]$. Thus

$$
\boxed{L_D^2=\frac c\beta=\frac{N}{\beta\sqrt{k^2+m^2+1/(4H^2)}}.}
$$

The eastward intrinsic branch $c>0$ is selected by decay away from the equator; choosing $c<0$ would make the meridional amplitude grow without bound. Although the squared [dispersion relation](../../../../dispersion-relation-split.md) has both [frequency](../../../../frequency.md) signs, a meridionally trapped [Kelvin wave](../../../../equatorial-kelvin-wave.md) has this one [phase-propagation](../../../../phase-velocity.md) direction.

For **short vertical [wavelengths](../../../../wavelength.md)**, $m^2\gg k^2+d^2$, so $\omega^2\simeq N^2k^2/m^2$, $c\simeq N/|m|$ and $L_D^2\simeq N/(\beta|m|)$. The wave is a slowly oscillating, [hydrostatic](../../../../hydrostatic-equilibrium.md) internal [gravity wave](../../../../gravity-wave-split.md) with strong vertical variation and relatively narrow trapping. Here $u\simeq-(m/k)w$ and $p'/\rho_0\simeq-(\omega m/k^2)w$; the [buoyancy](../../../../buoyancy.md) expression above remains valid.

For **long vertical [wavelengths](../../../../wavelength.md)**, $|m|\ll\sqrt{k^2+d^2}$, the exact limiting speed is $c=N/\sqrt{k^2+d^2}$. To obtain the stated height-controlled limit also requires long horizontal [wavelength](../../../../wavelength.md), $|k|H\ll1$. With both $|m|H\ll1$ and $|k|H\ll1$,

$$
\boxed{\omega\simeq2NHk,\qquad L_D^2\simeq\frac{2NH}{\beta}.}
$$

The finite [density scale height](../../../../scale-height.md) prevents the [hydrostatic](../../../../hydrostatic-equilibrium.md) $1/|m|$ [phase speed](../../../../phase-velocity.md) from diverging as $m\to0$. The polarizations tend to $u\simeq-iw/(2Hk)$, $\Phi\simeq-iNw/k$ and $b\simeq-iNw/(2Hk)$. Long vertical [wavelength](../../../../wavelength.md) alone at fixed large $kH$ would not justify $c=2NH$. In the opposite horizontally short limit the [frequency](../../../../frequency.md) approaches $N$ instead. The growth $e^{z/(2H)}$ compensates decreasing reference [density](../../../../density.md) in wave-energy [density](../../../../density.md); a radiating wave train is a local modal description, not a finite-total-energy eigenfunction over an infinite vertical domain.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
