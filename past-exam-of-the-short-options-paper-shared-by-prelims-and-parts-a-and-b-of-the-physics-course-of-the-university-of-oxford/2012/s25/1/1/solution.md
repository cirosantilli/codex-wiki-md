<h1 id="s25/1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Spectral irradiance](../../../../../spectral-irradiance.md) $F_\lambda$ is radiant power crossing unit area per unit wavelength, integrated over the relevant hemisphere with the projected-area factor: $F_\lambda=\int I_\lambda\cos\theta\,d\Omega$. Its units are $\mathrm{W\,m^{-2}}$ per unit wavelength; [spectral radiance](../../../../../spectral-radiance.md) $I_\lambda$ additionally refers to unit solid angle. For an isotropic outgoing hemisphere with [Planck function](../../../../../planck-function.md) $B_\lambda$, the integral is $F_\lambda=\pi B_\lambda$.

The vertical [optical depth](../../../../../optical-depth.md) above height $z$ is the dimensionless extinction integral

$$
\tau_\lambda(z)=\int_z^\infty n_a(z')\sigma_\lambda(z')\,dz',\qquad
\boxed{\frac{d\tau_\lambda}{dz}=-n_a\sigma_\lambda=-\kappa_\lambda\rho_a.}
$$

Here $z$ increases upward, $n_a$ is absorber [number density](../../../../../number-density.md), $\sigma_\lambda$ its absorption cross section, $\rho_a$ its [mass density](../../../../../density.md), and $\kappa_\lambda$ the absorption coefficient per unit absorber mass. Equivalently, using bulk air [density](../../../../../density.md) $\rho$ and absorber mass fraction $q_a$, $d\tau_\lambda/dz=-\kappa_\lambda q_a\rho$. The coefficient may depend on [temperature](../../../../../temperature-split.md), [pressure](../../../../../pressure-split.md) and wavelength. For purely absorbing gas, transmission along a ray is $e^{-\tau_{\rm ray}}$; scattering, if present, contributes to extinction and requires its own source term.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [1](../../1.md)
3. [S25](../../../s25.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
