# Compton recoil kinematics

↑ **Parent:** [Compton scattering](compton-scattering.md)

Choose the incident [photon](photon.md) direction as $+x$ and the plane of the [collision](collision.md) as the $xy$ plane, with the outgoing [photon](photon.md) above the $x$ axis. The [electron](electron.md) initially has zero [momentum](momentum-split.md). [Conservation of energy](conservation-of-energy.md) and [momentum conservation](momentum-conservation.md), using the relativistic [energy–momentum relation](energy-momentum-relation.md), give

$$
E+m_ec^2=E'+\sqrt{m_e^2c^4+c^2|\mathbf p_e|^2},
\qquad
c\mathbf p_e=(E-E'\cos\theta)\hat{\mathbf x}-E'\sin\theta\hat{\mathbf y}.
$$

Squaring the [electron](electron.md) [energy](energy-split.md) and the [momentum](momentum-split.md) magnitude in these two equations yields

$$
(m_ec^2+E-E')^2
=m_e^2c^4+E^2+E'^2-2EE'\cos\theta.
$$

Cancel common terms to obtain $m_ec^2(E-E')=EE'(1-\cos\theta)$. Division by $EE'>0$ gives $1/E'-1/E=(1-\cos\theta)/(m_ec^2)$. Substitution of $\lambda=hc/E$ proves both [Compton scattering](compton-scattering.md) formulas. Using the nonrelativistic approximation $T_e=|\mathbf p_e|^2/(2m_e)$ here would lose the exact relativistic result.

Let $\phi$ be the nonnegative [electron](electron.md) recoil angle below the incident direction. For $0<\theta<\pi$, the [vector components](coordinate-linear-algebra.md) above imply

$$
\tan\phi=\frac{E'\sin\theta}{E-E'\cos\theta}
=\frac{\cot(\theta/2)}{1+E/(m_ec^2)}.
$$

This assumes exactly the same initially stationary free [electron](electron.md) and single outgoing [photon](photon.md). At $\theta=\pi$, the [electron](electron.md) moves forward with $\phi=0$; at $\theta=0$ it stays at rest, so its recoil direction is undefined even though the limiting angle as $\theta\downarrow0$ is $\pi/2$. At $\theta=90^\circ$ in the chosen example, $c\mathbf p_e=(70,-61.566)\,\mathrm{keV}$ and $\phi\simeq41.33^\circ$.

<a id="image-photon-deflection-and-electron-recoil-in-compton-scattering"></a>
![](compton-photon-and-electron-momentum-vectors.png)

**[Figure 2](#image-photon-deflection-and-electron-recoil-in-compton-scattering). Photon deflection and electron recoil in Compton scattering**. Original $90^\circ$ example. Left: directions in the plane of the [collision](collision.md), with a labeled incident [photon](photon.md) source and an initially stationary [electron](electron.md); ray lengths are schematic. Right: [momentum](momentum-split.md) vectors multiplied by $c$, in $\mathrm{keV}$, with equal horizontal and vertical scales. The translated outgoing [photon](photon.md) [momentum](momentum-split.md) closes the triangle: $\mathbf p=\mathbf p_e+\mathbf p'$. No experimental trace is shown.

## ↑ Ancestors (5)

1. [Compton scattering](compton-scattering.md)
2. [Compton wavelength](compton-wavelength.md)
3. [Mathematical physics](mathematical-physics-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bothe-Geiger coincidence experiment](bothe-geiger-coincidence-experiment.md)
- [Thomson limit](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2019/section-b/b5/thomson-limit.md)
- [Thomson cross-section](thomson-cross-section.md)
