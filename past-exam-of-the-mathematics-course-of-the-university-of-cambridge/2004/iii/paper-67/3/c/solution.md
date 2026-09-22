<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is a genuine flux typo in the original PDF. A received bolometric [radiative flux](../../../../../../radiative-flux.md) must have inverse-square [luminosity distance](../../../../../../luminosity-distance.md), so the physically consistent [thermal bremsstrahlung](../../../../../../thermal-bremsstrahlung.md) expression is $S_X\propto d_L^{-2}\int n_e^2T_e^{1/2}\,dV$. The printed single power of $d_L$ cannot imply the requested [Hubble constant](../../../../../../hubble-constant.md) scaling.

For an approximately uniform, spherical [galaxy cluster](../../../../../../galaxy-cluster.md) let its depth be $\ell=q\theta d_A$, where $q$ is a fixed geometrical factor. With fixed profile coefficients $A,B$, the [Rayleigh-Jeans law](../../../../../../rayleigh-jeans-law.md) limit of the [thermal Sunyaev-Zeldovich effect](../../../../../../thermal-sunyaev-zeldovich-effect.md) and the bolometric X-ray [radiative flux](../../../../../../radiative-flux.md) give

$$
D\equiv|\Delta T_\gamma|=A n_eT_e\ell,\qquad
S_X=B\frac{n_e^2T_e^{1/2}\ell^3}{d_L^2}.
$$

Eliminate the electron [number density](../../../../../../number-density.md) and use $d_L=(1+z)^2d_A$:

$$
S_X=\frac B{A^2}\frac{D^2\ell}{T_e^{3/2}d_L^2}
=\frac{Bq}{A^2}\frac{D^2\theta}{T_e^{3/2}(1+z)^4d_A}.
$$

The [cluster distance from Sunyaev-Zeldovich and X-ray signals](../../../../../../cluster-distance-from-sunyaev-zeldovich-and-x-ray-signals.md) is consequently

$$
\boxed{d_A=\frac{Bq}{A^2}\frac{D^2\theta}{S_XT_e^{3/2}(1+z)^4}.}
$$

At low [cosmological redshift](../../../../../../cosmological-redshift.md), $d_A\simeq cz/H_0$, so

$$
\boxed{H_0\simeq\frac{c z A^2}{Bq}\frac{S_XT_e^{3/2}(1+z)^4}{D^2\theta}
\ \propto\ (\Delta T_\gamma)^{-2}}
$$

when the other observables and profile parameters are held fixed. With the PDF's literal $d_L^{-1}$ instead, $S_X/D^2\propto\ell/(T_e^{3/2}d_L)=q\theta/[T_e^{3/2}(1+z)^2]$, independent of distance: this explicitly shows why the correction is necessary.

Real [galaxy clusters](../../../../../../galaxy-cluster.md) are neither uniform nor generally spherical. The inferred depth depends on the ratio of [line of sight](../../../../../../line-of-sight.md) depth to transverse extent; elongation and orientation selection therefore bias the distance. [density](../../../../../../density.md) clumps enhance X-ray emission, which weights $n_e^2$, more than the [thermal Sunyaev-Zeldovich effect](../../../../../../thermal-sunyaev-zeldovich-effect.md), which weights $n_e$. An unmodelled [gas clumping factor](../../../../../../gas-clumping-factor.md) greater than one makes the inferred distance too small and the inferred [Hubble constant](../../../../../../hubble-constant.md) too large in this simple model. [Temperature](../../../../../../temperature.md) gradients and multiple thermal components bias the X-ray spectral temperature relative to the pressure-weighted [Compton y parameter](../../../../../../compton-y-parameter.md). Metals alter the cooling spectrum, and finite X-ray bands require a spectral and redshift correction to the bolometric approximation. Relativistic thermal corrections, the [kinetic Sunyaev-Zeldovich effect](../../../../../../kinetic-sunyaev-zeldovich-effect.md), radio sources and primary [Cosmic microwave background anisotropy](../../../../../../cosmic-microwave-background-anisotropy-split.md) contaminate the signal. Finally, calibration, angular-profile fitting and low-redshift [peculiar velocities](../../../../../../peculiar-velocity.md) affect the observables and the relation between measured redshift and expansion distance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
