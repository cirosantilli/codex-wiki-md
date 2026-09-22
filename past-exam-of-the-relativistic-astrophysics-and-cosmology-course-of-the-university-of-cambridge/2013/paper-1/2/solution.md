<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Friedmann-Lemaître-Robertson-Walker metric](../../../../friedmann-lemaitre-robertson-walker-metric.md) describes homogeneous, isotropic spatial slices. Here $t$ is [cosmic time](../../../../cosmic-time.md), equal to the [proper time](../../../../proper-time.md) of a [comoving observer](../../../../comoving-observer.md); $R(t)$ is the length-valued [scale factor](../../../../scale-factor-cosmology.md); and $\chi,\theta,\phi$ are dimensionless comoving radial, polar and azimuthal coordinates. The [speed of light](../../../../speed-of-light.md) is $c$, and

$$
S(\chi)=\begin{cases}\sin\chi&k=+1,\\\chi&k=0,\\\sinh\chi&k=-1,\end{cases}
$$

for positive, zero and negative [cosmological spatial curvature](../../../../spatial-curvature-of-an-flrw-universe.md). The convention used makes $ds^2$ a squared time interval, with signature $(+---)$; multiplying the metric by $c^2$ gives the more usual squared-length convention. At fixed $t$, radial proper length is $R(t)d\chi$, while a sphere has area $4\pi R^2(t)S^2(\chi)$.

[luminosity distance](../../../../luminosity-distance.md) is defined by $F=L/(4\pi d_L^2)$ for bolometric [radiative flux](../../../../radiative-flux.md) $F$ and intrinsic [luminosity](../../../../luminosity.md) $L$. Radial null propagation gives $d\chi=\pm c\,dt/R(t)$. Applying the same path integral to two successive wave crests gives $\Delta t_0/R_0=\Delta t_e/R_e$, hence $1+z=R_0/R_e$. Each [photon](../../../../photon.md) loses an [energy](../../../../energy-split.md) factor $1+z$, and their arrival rate loses another. For transparent propagation and isotropic emission,

$$
F=\frac{L}{4\pi R_0^2S^2(\chi)(1+z)^2},\qquad
\boxed{d_L=R_0S(\chi)(1+z)}.
$$

The two [redshift](../../../../redshift.md) factors have distinct physical origins; geometrical dilution alone is insufficient.

With $H=\dot R/R$, differentiating $1+z=R_0/R$ yields $dt/dz=-[(1+z)H(z)]^{-1}$. Therefore the radial [comoving coordinate](../../../../comoving-coordinate.md) is

$$
\chi=\int_{t_e}^{t_0}\frac{c\,dt}{R(t)}
=\boxed{\frac c{R_0}\int_0^z\frac{dz'}{H(z')}}.
$$

This is independent of any particular matter model; the [transverse comoving distance](../../../../transverse-comoving-distance.md) is $R_0S(\chi)$, which equals $R_0\chi$ only for flat space.

For [pressureless matter](../../../../pressureless-matter.md), the [continuity equation](../../../../continuity-equation.md) $\dot\rho_m+3H\rho_m=0$ integrates to $\rho_m=\rho_{m0}(R_0/R)^3=\rho_{m0}(1+z)^3$. The [cosmological constant](../../../../cosmological-constant.md) is kept separately from this matter density. In the flat [Friedmann equation](../../../../friedmann-equations.md), define

$$
\Omega_{\Lambda0}=\frac{\Lambda}{3H_0^2},\qquad
\Omega_{m0}=\frac{8\pi G\rho_{m0}}{3H_0^2}=1-\Omega_{\Lambda0}.
$$

The [flat dust-vacuum Hubble parameter](../../../../flat-dust-vacuum-hubble-parameter.md) is therefore

$$
\boxed{H(z)=H_0\sqrt{(1-\Omega_{\Lambda0})(1+z)^3+\Omega_{\Lambda0}}}.
$$

In the equation's convention $\rho_m$ is mass-equivalent [energy density](../../../../energy-density.md) and $\Lambda$ has units $\mathrm{s^{-2}}$; the geometrical [cosmological constant](../../../../cosmological-constant.md) convention instead writes $c^2\Lambda_{\rm geom}$. The model contains dust and [vacuum energy](../../../../vacuum-energy.md) with negligible [radiation](../../../../radiation.md) over the relevant late epochs: “matter-dominated” here does not require matter to exceed [vacuum energy](../../../../vacuum-energy.md) today.

The [cosmic microwave background](../../../../cosmic-microwave-background-split.md) supplies a standard ruler through its acoustic scale: the angular positions of the [Cosmic microwave background acoustic peaks](../../../../cosmic-microwave-background-acoustic-peak.md) constrain [cosmological spatial curvature](../../../../spatial-curvature-of-an-flrw-universe.md), while their relative heights constrain matter and [baryon](../../../../baryon.md) densities. Together with independent distance information, these favour a nearly flat [Lambda-CDM model](../../../../lambda-cdm-model.md) containing substantial [cold dark matter](../../../../cold-dark-matter.md) and [vacuum energy](../../../../vacuum-energy.md). The [cosmic microwave background](../../../../cosmic-microwave-background-split.md) alone has a geometrical degeneracy between parameters affecting distance to last scattering; its analysis also includes early [radiation](../../../../radiation.md), which the late-time formula above omits. The nine-year [WMAP](../../../../wilkinson-microwave-anisotropy-probe.md) results were already available as a December 2012 preprint.[Version 1 abstract: combined-data curvature constraint and consistency with the six-parameter Lambda-CDM model](../../../../nine-year-wilkinson-microwave-anisotropy-probe-wmap-observations-final-maps-and-results-by-c-l-bennett-and-others.md)

A standardized [Type Ia supernova](../../../../type-ia-supernova.md) at appreciable [redshift](../../../../redshift.md) is fainter, hence farther in [luminosity distance](../../../../luminosity-distance.md), than in a matter-only [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md) with the same local expansion scale. Fitting the supernova [Hubble diagram](../../../../hubble-diagram.md) supports late acceleration; in flat dust plus vacuum, $q_0=\Omega_{m0}/2-\Omega_{\Lambda0}$ is negative for $\Omega_{\Lambda0}>1/3$. Light-curve and colour corrections, extinction, calibration, selection bias and possible population evolution must be controlled. The supernova evidence and [cosmic microwave background](../../../../cosmic-microwave-background-split.md) constraints are complementary; together they favour this model without proving that every alternative dark-energy model is impossible.[Abstract and cosmological fits of the supernova distance-redshift relation](../../../../observational-evidence-from-supernovae-for-an-accelerating-universe-and-a-cosmological-constant-by-adam-riess-and-others.md)[Abstract and joint matter-density/cosmological-constant fits](../../../../measurements-of-omega-and-lambda-from-42-high-redshift-supernovae-by-saul-perlmutter-and-others.md)

For the final comparison, assume $z>0$, a common $H_0$ and $0<\Omega_{\Lambda0}<1$ in model (a). Then

$$
H_c=H_0,\qquad H_a=H_0\sqrt{(1-\Omega_{\Lambda0})(1+z)^3+\Omega_{\Lambda0}},\qquad
H_b=H_0(1+z)^{3/2}.
$$

Thus $H_c<H_a<H_b$ and the integrands obey $1/H_b<1/H_a<1/H_c$. Because all three models are flat, compare the normalization-independent distance $R_0\chi=c\int dz'/H(z')$, rather than separately normalized coordinates. The [luminosity-distance ordering of flat dust-vacuum universes](../../../../luminosity-distance-ordering-of-flat-dust-vacuum-universes.md) is $d_{L,b}<d_{L,a}<d_{L,c}$, hence

$$
\boxed{F_b>F_a>F_c}.
$$

Model (b) gives the largest received flux, model (c) the smallest. Equalities replace the strict ordering at the endpoint values of the vacuum fraction; all have the same leading local [Hubble law](../../../../hubble-s-law.md) as $z\to0$.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
