# Rayleigh optical gradient force

↑ **Parent:** [Optical gradient force](optical-gradient-force.md)

The [geometrical optics](geometrical-optics-split.md) account of an [optical trap](optical-tweezers.md) adds the [momentum](momentum-split.md) flux changes of refracted and reflected [light rays](light-ray.md). It applies when the bead is large compared with the surrounding medium's [wavelength](wavelength.md). When the bead is much smaller, an induced [electric dipole](electric-dipole.md) gives a different approximation. For a homogeneous [dielectric](dielectric.md) [sphere](sphere.md) of [radius](radius.md) $a$, define $\mathbf p(t)=\operatorname{Re}[\alpha\mathbf E_0e^{-i\omega t}]$, with $\mathbf E_0$ the peak complex [electric field](electric-field-split.md) and $\alpha$ its SI [polarizability](electric-polarizability.md). In a transparent, nonmagnetic, nondispersive host,

$$
\epsilon_m=\epsilon_0 n_m^2,\qquad
\alpha=4\pi\epsilon_m a^3\frac{n_p^2-n_m^2}{n_p^2+2n_m^2},\qquad
I=\frac12n_m\epsilon_0c|\mathbf E_0|^2,
$$

where $n_p,n_m$ are particle and host [refractive indices](refractive-index.md), $I$ is cycle-averaged [light intensity](light-intensity.md), $\epsilon_0$ is the [vacuum permittivity](vacuum-permittivity.md) and $c$ is the [speed of light](speed-of-light.md). The quasistatic [electric dipole](electric-dipole.md) approximation requires $2\pi n_ma/\lambda_0\ll1$, with $\lambda_0$ the [vacuum](vacuum.md) [wavelength](wavelength.md), and a field nearly uniform across the bead.

For real quasistatic $\alpha$, building an induced [electric dipole](electric-dipole.md) gives instantaneous [potential energy](potential-energy.md) $-\alpha E^2/2$. Averaging over one optical cycle gives

$$
U_{\mathrm{grad}}=-\frac14\alpha|\mathbf E_0|^2,
\qquad \mathbf F_{\mathrm{grad}}=-\nabla U_{\mathrm{grad}}
=\frac{\alpha}{2n_m\epsilon_0c}\nabla I.
$$

Thus $n_p>n_m$ gives positive [polarizability](electric-polarizability.md) and attraction toward larger [light intensity](light-intensity.md); $n_p<n_m$ reverses this contribution. The factor $1/4$ uses a peak field: substituting a [root mean square](root-mean-square.md) field without changing that factor would halve the [force](force-split.md) incorrectly. Dimensionally $\alpha|E_0|^2$ is [energy](energy-split.md), so its [gradient](gradient.md) is [force](force-split.md).

This leading conservative term does not remove the [optical scattering force](optical-scattering-force.md). Even a nonabsorbing induced [electric dipole](electric-dipole.md) reradiates [light](light.md): at fixed [wavelength](wavelength.md) and index contrast, its [Rayleigh scattering cross-section](rayleigh-scattering-by-a-small-sphere.md) scales as $a^6$, while $\alpha$ scales as $a^3$. A smaller bead can therefore improve the ratio of gradient to scattering [forces](force-split.md) while weakening the well relative to $k_BT$, where $k_B$ is the [Boltzmann constant](boltzmann-constant.md) and $T$ the [temperature](temperature-split.md). Optical [force balance](force-balance.md) and resistance to thermal escape are separate questions. Intermediate bead sizes require a wave-scattering calculation; neither a ray calculation nor this small-dipole expression is uniformly valid there.

## ↑ Ancestors (6)

1. [Optical gradient force](optical-gradient-force.md)
2. [Optical tweezers](optical-tweezers.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
