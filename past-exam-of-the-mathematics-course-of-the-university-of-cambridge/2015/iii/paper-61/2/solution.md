<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Treat the features in the [QSO](../../../../../quasar.md) spectrum as [Lyman-alpha absorption](../../../../../lyman-alpha-absorption.md) and use the [cosmological wavelength-redshift relation](../../../../../cosmological-wavelength-redshift-relation.md) to convert their spacing into $\Delta z=304/1216=0.25$. In the specified flat matter-plus-cosmological-constant model,

$$
H(3)=H_0\sqrt{\Omega_m(1+3)^3+\Omega_\Lambda}=70\sqrt{16.75}\simeq286.5\,\mathrm{km\,s^{-1}\,Mpc^{-1}}.
$$

A local radial interval has comoving length $d\chi=c\,dz/H(z)$ and proper length $dl=d\chi/(1+z)$. Evaluating the mean interval locally at $z=3$ gives the [proper absorber separation from a wavelength interval](../../../../../proper-absorber-separation-from-a-wavelength-interval.md)

$$
\boxed{\ell\simeq\frac{c\Delta z}{(1+z)H(z)}\simeq65.4\,\mathrm{Mpc}.}
$$

The corresponding comoving interval is about $262\,\mathrm{Mpc}$. We neglect peculiar-velocity shifts and treat $H$ as approximately constant over one mean interval.

The proper number density is $n_p=(1+z)^3n_{\rm gal}=179.2\,\mathrm{Mpc^{-3}}$. To compute the [mean projected area of a randomly oriented thin disc](../../../../../mean-projected-area-of-a-randomly-oriented-thin-disc.md), note that a disc whose normal makes angle $i$ to the sightline has projected area $\pi R_d^2|\cos i|$. Isotropic normals have

$$
\langle|\cos i|\rangle=\frac12\int_{-1}^{1}|\mu|\,d\mu=\frac12.
$$

For independent intersections with fully covering [thin discs](../../../../../thin-disk.md), the [mean free path through randomly oriented disc absorbers](../../../../../mean-free-path-through-randomly-oriented-disc-absorbers.md) is $\ell^{-1}=n_p\pi R_d^2/2$. Thus

$$
\boxed{R_d=\left(\frac{2}{\pi n_p\ell}\right)^{1/2}\simeq7.37\,\mathrm{kpc}.}
$$

All radii here are proper radii at the absorber epoch. The projected-area average is over the underlying orientation distribution; it already accounts for the larger intersection probability of face-on discs.

The [cosmic baryon fraction](../../../../../cosmic-baryon-fraction.md) is $f_b=\Omega_b/\Omega_m=0.2$, so the disc mass is $M_d=f_dM_h$ with $f_d=f_b/4=0.05$. Define $v_{\rm vir}^2=GM_h/R_{\rm vir}$. Disc gravity depends on its radial mass profile, which has not been specified. Parameterize its edge circular speed by $v_d^2=C_dGM_d/R_d$ and use $C_d=1$ for a centrally concentrated disc in a monopole approximation at its outer edge. The angular-momentum condition gives

$$
R_dv_d=0.1R_{\rm vir}v_{\rm vir},\qquad v_d^2=C_df_d\frac{R_{\rm vir}}{R_d}v_{\rm vir}^2.
$$

Combining the equations yields the [angular-momentum-conserving self-gravitating disc radius](../../../../../angular-momentum-conserving-self-gravitating-disc-radius.md)

$$
\boxed{\frac{R_{\rm vir}}{R_d}=\frac{C_df_d}{0.1^2}=5C_d.}
$$

For the stated $C_d=1$ choice, **$R_{\rm vir}\simeq36.8\,\mathrm{kpc}$** and $v_d=0.5v_{\rm vir}$. The factor $C_d$ makes explicit the otherwise undetermined disc-profile dependence; an enclosed-mass formula is not exact for an arbitrary flattened disc.

To determine the halo speed, a virial-density convention is also needed. Choose a spherical overdensity $\Delta_v=200$ relative to the [critical density](../../../../../critical-density.md) at $z=3$:

$$
M_h=\frac{4\pi}{3}\Delta_v\rho_{\rm crit}(3)R_{\rm vir}^3,\qquad \rho_{\rm crit}(3)=\frac{3H^2(3)}{8\pi G}.
$$

The [virial velocity of a spherical-overdensity halo](../../../../../virial-velocity-of-a-spherical-overdensity-halo.md) then obeys

$$
\boxed{v_{\rm vir}=H(3)R_{\rm vir}\sqrt{\frac{\Delta_v}{2}}\simeq1.06\times10^2\,\mathrm{km\,s^{-1}}.}
$$

The nearly matter-dominated spherical-collapse choice $\Delta_v\simeq18\pi^2$ instead gives about $99.5\,\mathrm{km\,s^{-1}}$. More generally the numerical radius and velocity scale respectively as $C_d$ and $C_d\sqrt{\Delta_v/200}$. With $G\simeq4.30\times10^{-6}\,\mathrm{kpc\,(km\,s^{-1})^2}M_\odot^{-1}$, the adopted model has $M_h\simeq9.5\times10^{10}M_\odot$ and $M_d\simeq4.8\times10^9M_\odot$; these reproduce the edge speed and the specified angular momentum.

The calculation assumes homogeneous, unclustered intersections, one detectable absorption feature per disc crossing, unit neutral-gas covering factor, isotropic orientations, universal halo baryon fraction and conservation of the specified edge specific angular momentum. It assumes the halo is virialized at the absorber epoch and neglects its inner gravity as instructed. The extra profile and overdensity choices are necessary to turn the geometric and angular-momentum constraints into unique numerical halo properties.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
