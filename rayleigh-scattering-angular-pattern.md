# Rayleigh scattering angular pattern

↑ **Parent:** [Rayleigh scattering](rayleigh-scattering.md)

For incident [unpolarized light](unpolarized-light.md) and the isotropic [electric dipole](electric-dipole.md) response of [Rayleigh scattering by a small sphere](rayleigh-scattering-by-a-small-sphere.md), let $\theta$ be the angle between the incident beam's propagation direction and the outgoing direction. The [differential scattering cross-section](differential-scattering-cross-section.md) and its relative angular pattern are

$$
\frac{d\sigma}{d\Omega}=\frac{3\sigma}{16\pi}(1+\cos^2\theta),\qquad F(\theta)=\frac{1+\cos^2\theta}{2},
$$

where $d\Omega$ is an element of [solid angle](solid-angle.md). Averaging over the two transverse directions of incident [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) gives this pattern. Forward scattering at $0^\circ$ and backward scattering at $180^\circ$ are equally strong: $F=1$. Sideways scattering at $90^\circ$ is weakest, but nonzero: $F=1/2$. [Fitzpatrick, Thomson Scattering, equations 1283–1287: averaging the dipole angular pattern](https://farside.ph.utexas.edu/teaching/jk1/lectures/node107.html).

<a id="image-rayleigh-scattering-angular-pattern-for-incident-unpolarized-light-measured-from-the-incident-beam"></a>
![](rayleigh-angular-scattering.png)

**[Figure 13](#image-rayleigh-scattering-angular-pattern-for-incident-unpolarized-light-measured-from-the-incident-beam). Rayleigh scattering angular pattern for incident unpolarized light, measured from the incident beam**. The plotted radial coordinate is $F(\theta)$, a relative [differential scattering cross-section](differential-scattering-cross-section.md), rather than the distance travelled by [light](light.md). The incident propagation axis points right: $0^\circ$ is forward, $180^\circ$ backward, and $90^\circ$ sideways. Rotating this plane about the incident axis gives the three-dimensional pattern.

The normalization is consistent because

$$
\int(1+\cos^2\theta)\,d\Omega=2\pi\int_0^\pi(1+\cos^2\theta)\sin\theta\,d\theta=\frac{16\pi}{3}.
$$

Thus integrating $d\sigma/d\Omega$ gives the total [Rayleigh scattering cross-section](rayleigh-scattering-by-a-small-sphere.md) $\sigma$. The plotted $F$ has maximum one; it is not itself normalized to unit [solid angle](solid-angle.md) integral.

For a single [electric dipole](electric-dipole.md) driven by incident [linear polarization](linear-polarization.md), the [angular distribution of electric dipole radiation](angular-distribution-of-electric-dipole-radiation.md) instead has a $\sin^2\alpha$ factor, where $\alpha$ is measured from the [electric dipole moment](electric-dipole-moment.md) direction, parallel to the incident [electric field](electric-field.md). That direction is perpendicular to the incident beam. Confusing $\alpha$ with the beam angle $\theta$ would incorrectly predict zero forward scattering. Averaging the dipole patterns over incident [unpolarized light](unpolarized-light.md) yields the displayed $F(\theta)$.

## ↑ Ancestors (6)

1. [Rayleigh scattering](rayleigh-scattering.md)
2. [Electromagnetic radiation](electromagnetic-radiation.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Rayleigh scattering angular pattern](rayleigh-scattering-angular-pattern.md)
