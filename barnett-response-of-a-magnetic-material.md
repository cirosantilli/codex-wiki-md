# Barnett response of a magnetic material

↑ **Parent:** [Barnett effect](barnett-effect.md)

The two-state calculation is not a general formula for a [ferromagnet](ferromagnet.md). [Exchange interactions](exchange-interaction.md), [magnetic domains](magnetic-domain.md), [magnetic domain-wall pinning](magnetic-domain-wall-pinning.md), [magnetic anisotropy](magnetic-anisotropy.md), and [hysteresis](hysteresis.md) can determine which response is accessible. Both [spin angular momentum](spin.md) and [orbital angular momentum](orbital-angular-momentum.md) can contribute; a single constant [gyromagnetic ratio](gyromagnetic-ratio.md) may be only a restricted effective description. Rotation sets an internal bias, while the material and its preparation determine [magnetization](magnetization.md). The [Barkhausen effect](barkhausen-effect.md) illustrates why a smooth bias can produce jumps instead of the toy smooth curve.

For a limited, reversible, isotropic linear model, suppose the same intrinsic [volume magnetic susceptibility](volume-magnetic-susceptibility.md) $\chi_v$ responds to the applied bias and to $B_\Omega/\mu_0$. For a uniformly magnetized [ellipsoid](ellipsoid.md) along a principal axis, include its [demagnetizing factor](demagnetizing-factor.md) $N_d$:

$$
H_{\rm int}=H_{\rm app}-N_dM_z,\qquad
M_z=\chi_v\left(H_{\rm app}-N_dM_z+\frac{B_\Omega}{\mu_0}\right).
$$

Solving this [linear equation](linear-equation.md) yields

$$
M_z=\frac{\chi_v}{1+N_d\chi_v}
\left(H_{\rm app}+\frac{\Omega}{\mu_0\gamma}\right).
$$

Here $H_{\rm int}$ and $H_{\rm app}$ are actual [magnetic field intensities](magnetic-field-intensity.md); the added rotational bias is an equivalent drive in the constitutive response. In [SI](international-system-of-units.md), dimensionless $\chi_v$ multiplies an intensity in $\mathrm{A/m}$, so $M_z=\chi_v\Omega/\gamma$ would omit $\mu_0$ and have the wrong units. A susceptibility defined instead as $\partial M/\partial B$ has different units. State the convention before comparing formulas.

At zero applied [magnetic field intensity](magnetic-field-intensity.md), a stipulated $\chi_v=3$ gives prefactor $3/2$ in a [sphere](sphere.md), with $N_d=1/3$, and a prefactor approaching $3$ in a long axial [ellipsoid](ellipsoid.md). This is a geometry check of the assumed linear model. A real cylinder does not have an exactly uniform [demagnetizing field](demagnetizing-field.md), and an irreversible [ferromagnet](ferromagnet.md) cannot in general be represented by this single linear equation. Inferring an intrinsic [gyromagnetic ratio](gyromagnetic-ratio.md) requires an independently calibrated material response and a geometry-dependent conversion of the measured stray [magnetic field](magnetic-field-split.md).

## ↑ Ancestors (7)

1. [Barnett effect](barnett-effect.md)
2. [Magnetic dipole moment](magnetic-dipole-moment.md)
3. [Magnetic vector potential](magnetic-vector-potential.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
