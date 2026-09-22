# Neutron scattering kinematics

↑ **Parent:** [Neutron scattering](neutron-scattering.md)

Treat the incident and outgoing [neutrons](neutron-split.md) as free [nonrelativistic particles](nonrelativistic-particle.md) outside the specimen. Their [wave vectors](wavevector.md), [de Broglie wavelengths](de-broglie-wavelength.md), [momenta](momentum-split.md) and [kinetic energies](kinetic-energy.md) obey

$$
k_i=\frac{2\pi}{\lambda_i},\qquad k_f=\frac{2\pi}{\lambda_f},\qquad
\mathbf p_i=\hbar\mathbf k_i,\qquad \mathbf p_f=\hbar\mathbf k_f,\qquad
E_{i,f}=\frac{\hbar^2 k_{i,f}^2}{2m_n}.
$$

Here $k_i=|\mathbf k_i|$, $k_f=|\mathbf k_f|$, $m_n$ is the [neutron](neutron-split.md) [mass](mass.md), and $\hbar=h/(2\pi)$ uses the [Planck constant](planck-constant.md). Subtracting the outgoing projectile quantities from the incoming ones gives the [momentum transfer](momentum-transfer.md) and [energy](energy-split.md) delivered to the specimen:

$$
\Delta\mathbf p=\hbar\mathbf Q,\qquad
\mathbf Q=\mathbf k_i-\mathbf k_f,\qquad
\Delta E=E_i-E_f=\hbar\omega.
$$

Thus $\mathbf Q$ has units of inverse [length](length.md), rather than [momentum](momentum-split.md). A positive $\omega$ means the specimen gains [energy](energy-split.md); negative $\omega$ means it supplies [energy](energy-split.md) to the [neutron](neutron-split.md). If the angle between incident and outgoing propagation directions is $2\theta$, the [law of cosines](law-of-cosines.md) gives

$$
Q^2=k_i^2+k_f^2-2k_i k_f\cos(2\theta).
$$

Knowing the detector angle alone therefore leaves $Q$ undetermined unless the outgoing [energy](energy-split.md) is known or an [elastic scattering](elastic-scattering.md) assumption is justified.

For a reproducible unit conversion choose $m_n=1.67492750056\times10^{-27}\,\mathrm{kg}$, $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$ and $1\,\mathrm{eV}=1.602176634\times10^{-19}\,\mathrm J$. The first is a recommended central value; the latter two conversions are exact.[2022 CODATA table: neutron mass, Planck constant and electron volt](fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others.md) With $1$ [ångström](angstrom.md) equal to $10^{-10}\,\mathrm m$ and $1\,\mathrm{meV}=10^{-3}$ [electronvolts](electronvolt.md), substitution into $E=h^2/(2m_n\lambda^2)$ gives

$$
E\,[\mathrm{meV}]=\frac{81.8042}{\bigl(\lambda\,[\mathrm{\mathring A}]\bigr)^2}
=2.07212\bigl(k\,[\mathrm{\mathring A}^{-1}]\bigr)^2.
$$

Square brackets here mean the numerical value in the indicated unit. For an original chosen example, $\lambda_i=2$ [ångströms](angstrom.md) and $\lambda_f=2.5$ [ångströms](angstrom.md) give $E_i\simeq20.451\,\mathrm{meV}$, $E_f\simeq13.089\,\mathrm{meV}$ and $\hbar\omega\simeq7.362\,\mathrm{meV}$. At $2\theta=60^\circ$, $Q\simeq2.879\,\mathrm{\mathring A}^{-1}$. These values stipulate an allowed projectile geometry; they do not assert that any particular specimen has an excitation there.

**Table of contents**

- [Perpendicular neutron recoil and phonon absorption](perpendicular-neutron-recoil-and-phonon-absorption.md)

## ↑ Ancestors (8)

1. [Neutron scattering](neutron-scattering.md)
2. [Neutron](neutron-split.md)
3. [Nucleon](nucleon.md)
4. [Baryon](baryon.md)
5. [Hadron](hadron.md)
6. [Subatomic particle](subatomic-particle.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Neutron diffraction](neutron-diffraction.md)
