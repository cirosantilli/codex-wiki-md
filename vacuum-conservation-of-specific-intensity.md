# Vacuum conservation of specific intensity

↑ **Parent:** [Spectral radiance](spectral-radiance.md)

In a transparent, stationary [vacuum](vacuum.md) with [Euclidean geometry](euclidean-geometry.md) and observers at rest in the same frame, the [radiative transfer equation](radiative-transfer-equation.md) has zero absorption and emission, so $dI_\nu/ds=0$ along a [light ray](light-ray.md). The same [specific intensity](spectral-radiance.md) reaches the observer without geometric dilution. More generally, $I_\nu/\nu^3$ is a [Lorentz invariant](lorentz-invariance.md); collisionless propagation preserves this ratio along a ray even with gravitational or cosmological [redshift](redshift.md), rather than preserving $I_\nu$ at shifted [frequencies](frequency.md). [John Peacock, Radiation and Matter, 2018–2019, §4.1, Conservation of intensity and equation (140)](https://www.roe.ac.uk/japwww/teaching/ram5/ram5_2018.pdf#page=27).

The elementary geometry is instructive. Two facing surface elements separated by distance $s$ exchange spectral [radiant flux](radiant-flux.md)

$$
d^3\Phi=I_\nu\frac{\cos\theta_1\cos\theta_2}{s^2}\,dA_1\,dA_2\,d\nu.
$$

The receiver subtends $d\Omega_2=\cos\theta_2\,dA_2/s^2$ at the source. Describing that same traveling beam at the receiver instead uses $d\Omega_1=\cos\theta_1\,dA_1/s^2$. Both descriptions have identical geometric factors, so conservation of its [radiant flux](radiant-flux.md) gives equal [specific intensities](spectral-radiance.md) at the two ends. This compares the same propagation direction at both ends, not emission in the opposite direction.

A uniform source remains equally bright per resolved direction under these assumptions, but occupies a smaller apparent [solid angle](solid-angle.md) farther away. For a small source of [projected area](projected-area.md) $A_\perp$ at distance $d$ and a small receiver facing it, [irradiance](irradiance.md) is approximately $E=L\Omega_{\rm source}\simeq LA_\perp/d^2$. The [radiant flux](radiant-flux.md) intercepted by receiver [area](surface-area.md) $A_d$ is approximately $EA_d$. With $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$, $A_\perp=0.020\,\mathrm{m^2}$ and $A_d=10^{-4}\,\mathrm{m^2}$, distances $10$ and $20\,\mathrm m$ give $E\simeq0.002$ and $0.0005\,\mathrm{W\,m^{-2}}$, and received [radiant fluxes](radiant-flux.md) of $0.20$ and $0.050\,\mu\mathrm W$. The [inverse-square law](inverse-square-law.md) concerns collected radiation from the whole source; $L$ remains $10$ at either distance.

## ↑ Ancestors (7)

1. [Spectral radiance](spectral-radiance.md)
2. [Radiance](radiance.md)
3. [Radiometry](radiometry.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/4/c/solution.md)
- [Radiance](radiance.md)
