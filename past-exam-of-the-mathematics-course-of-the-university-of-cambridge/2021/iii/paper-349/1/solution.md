<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Interstellar dust](../../../../../interstellar-dust.md) both hides and reveals galaxies. Absorption and scattering remove short-wavelength photons from a line of sight, causing [interstellar extinction](../../../../../interstellar-extinction.md), reddening, anisotropic scattering, and polarization. These effects obscure embedded [star formation](../../../../../star-formation.md), bias luminosities, colours, stellar masses, and star-formation rates, and can make an edge-on or dusty galaxy appear older and fainter. Dust also converts absorbed ultraviolet and optical power into far-infrared and submillimetre [thermal radiation](../../../../../thermal-radiation.md). That reradiation exposes otherwise hidden star formation, constrains dust temperature and mass, and helps map cold molecular material; polarization traces magnetic-field orientation. Grain surfaces also catalyse molecular-hydrogen formation, while photoelectric emission from grains heats interstellar gas.

One spherical grain has emitting area $4\pi a^2$. Since isotropic [blackbody](../../../../../blackbody.md) intensity $B_\nu$ gives surface flux $\pi B_\nu$, its spectral luminosity is

$$
L_{\nu,g}=4\pi^2a^2Q_\nu B_\nu(T).
$$

For $N=M_d/m_d$ optically thin grains at distance $D$, the [inverse-square law](../../../../../inverse-square-law.md) gives

$$
F_\nu=\frac{NL_{\nu,g}}{4\pi D^2}
=\frac{M_d}{m_d}\frac{\pi a^2Q_\nu B_\nu}{D^2}.
$$

Defining the grain [mass absorption coefficient](../../../../../mass-absorption-coefficient.md)

$$
\kappa_\nu=\frac{\pi a^2Q_\nu}{m_d},
$$

the [optically thin dust-mass estimator](../../../../../optically-thin-dust-mass-estimator.md) is

$$
\boxed{M_d=\frac{F_\nu D^2}{\kappa_\nu B_\nu(T)}
=\frac{m_dF_\nu D^2}{\pi a^2Q_\nu B_\nu(T)}}.
$$

For a constant source function and no incident background, the [radiative transfer equation](../../../../../radiative-transfer-equation.md) integrates to

$$
\boxed{I_\nu(\tau_\nu)=B_\nu(T)(1-e^{-\tau_\nu})}.
$$

If the cloud subtends [solid angle](../../../../../solid-angle.md) $\Omega$, uniform intensity gives

$$
F_\nu=\Omega B_\nu(T)(1-e^{-\tau_\nu}).
$$

The physical projected area is $A=\Omega D^2$. Its grain column density is $N/A=M_d/(m_d\Omega D^2)$, so the [dust optical depth](../../../../../dust-optical-depth.md) is

$$
\tau_\nu=\frac{M_d\pi a^2Q_\nu}{m_d\Omega D^2}
=\frac{\kappa_\nu M_d}{\Omega D^2}.
$$

Eliminating $\tau_\nu$ gives the finite-optical-depth result

$$
\boxed{M_d=-\frac{\Omega D^2}{\kappa_\nu}
\log\left(1-\frac{F_\nu}{\Omega B_\nu(T)}\right)}.
$$

It requires $F_\nu<\Omega B_\nu$, as demanded by the [blackbody](../../../../../blackbody.md) brightness limit. When $\tau_\nu\ll1$, $1-e^{-\tau_\nu}=\tau_\nu+O(\tau_\nu^2)$, so $F_\nu\simeq\Omega B_\nu\tau_\nu=\kappa_\nu M_dB_\nu/D^2$ and the result reduces to the optically thin estimator.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
