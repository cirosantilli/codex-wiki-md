<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a characteristic midplane [temperature](../../../../../../temperature.md) $T$, density $\rho$ and [disk scale height](../../../../../../disk-scale-height.md) $H$. For an [ideal gas](../../../../../../ideal-gas.md) of fixed composition, dominant [gas pressure](../../../../../../gas-pressure.md) gives $c_s^2\propto T$, where $c_s$ is the [sound speed](../../../../../../speed-of-sound.md). Vertical [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) and the [alpha disk](../../../../../../alpha-disk.md) prescription give

$$
H\sim\frac{c_s}{\Omega}\propto\frac{T^{1/2}}\Omega,\qquad
\rho\sim\frac\Sigma H\propto\Sigma\Omega T^{-1/2},\qquad
\nu\sim\alpha c_sH\propto\frac{\alpha T}\Omega.
$$

Numerical factors in the vertical averaging do not affect the exponents. The stipulated [opacity](../../../../../../opacity.md) becomes

$$
\kappa\propto(\Sigma\Omega T^{-1/2})^{-3/2}T^{5/4}
=\Sigma^{-3/2}\Omega^{-3/2}T^2.
$$

For an optically thick, radiatively efficient disk, [radiative diffusion](../../../../../../radiative-diffusion.md) gives a cooling rate per unit area proportional to $T^4/(\kappa\Sigma)$. The viscous heating rate is proportional to $\nu\Sigma\Omega^2$. Thus

$$
Q^-\propto\Sigma^{1/2}\Omega^{3/2}T^2,\qquad
Q^+\propto\alpha\Sigma\Omega T.
$$

Equating heating and cooling gives $T\propto\alpha\Sigma^{1/2}\Omega^{-1/2}$, so

$$
\nu\propto\alpha^2\Sigma^{1/2}\Omega^{-3/2}.
$$

At fixed $\alpha$ and central mass, $\Omega\propto R^{-3/2}$. Therefore the [gas-pressure alpha disk with inverse-density opacity](../../../../../../gas-pressure-alpha-disk-with-inverse-density-opacity.md) satisfies

$$
\boxed{\nu\propto\Sigma^{1/2}R^{9/4}.}
$$

For [thermal stability of an accretion disk](../../../../../../thermal-stability-of-an-accretion-disk.md), perturb $T$ at fixed $R$ and $\Sigma$, since the thermal adjustment is faster than radial mass redistribution. The logarithmic heating and cooling slopes are respectively one and two. At equilibrium, a fractional [temperature](../../../../../../temperature.md) increase therefore makes the excess heating $Q^+-Q^-$ decrease, and the disk cools back. Thus **the local thermal equilibrium is stable** within the assumed gas-pressure, radiative-diffusion closure.

For [viscous stability of an accretion disk](../../../../../../viscous-stability-of-an-accretion-disk.md), use the thermally equilibrated relation between [viscosity](../../../../../../dynamic-viscosity.md) and [surface density](../../../../../../surface-density-of-a-disk.md). It gives

$$
\nu\Sigma\propto\Sigma^{3/2}R^{9/4},\qquad
\left.\frac{\partial(\nu\Sigma)}{\partial\Sigma}\right|_R>0.
$$

Locally freezing the background radius in the [Keplerian viscous diffusion equation](../../../../../../keplerian-viscous-diffusion-equation.md), a short radial [Fourier mode](../../../../../../fourier-mode.md) has growth rate $-3k_R^2\partial_\Sigma(\nu\Sigma)<0$. Density enhancements diffuse rather than grow, so **the disk is locally viscously stable** as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
