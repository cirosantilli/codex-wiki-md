<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $M_h,R_h$ describe the halo and let $v=v_{\rm vir}$. The [cosmic baryon fraction](../../../../../cosmic-baryon-fraction.md) is $f_b=\Omega_b/\Omega_m=0.20$, so the specified settled fraction gives $M_d=0.10M_h$. The [specific angular momentum](../../../../../specific-angular-momentum.md) constraint at the disk edge is

$$
R_dv_d=f_jR_hv,\qquad f_j=0.10.
$$

To infer an actual [circular speed](../../../../../circular-speed.md) one must specify the disk's radial mass distribution: [enclosed mass does not determine a disc rotation curve](../../../../../enclosed-mass-does-not-determine-a-disc-rotation-curve.md). Introduce a finite geometry coefficient $\kappa$ by $v_d^2=\kappa GM_d/R_d$. A rounded, centrally concentrated disk permits a monopole estimate $\kappa\simeq1$ at its outer edge; it is an explicit approximation, not the spherical shell theorem applied exactly to a razor-thin disk. Ignore the force of the unsettled baryons as well as the [dark matter](../../../../../dark-matter.md) within the disk. Using $v^2=GM_h/R_h$, the [angular-momentum estimate of a self-gravitating galactic disk](../../../../../angular-momentum-estimate-of-a-self-gravitating-galactic-disk.md) gives

$$
\boxed{\frac{R_d}{R_h}=\frac{f_j^2}{\kappa f_d}=\frac{0.10}{\kappa},\qquad
\frac{v_d}{v}=\frac{\kappa f_d}{f_j}=\kappa,\qquad f_d=0.10.}
$$

An exact disk answer cannot be fixed by total disk mass alone; the dependence on $\kappa$ records that missing input.

For the numerical [virial radius of a dark-matter halo](../../../../../virial-radius-of-a-dark-matter-halo.md), adopt mean density $\Delta_c=200$ times the [critical density](../../../../../critical-density.md) at the formation epoch. This conventional definition gives

$$
M_h=\frac{4\pi}3\Delta_c\frac{3H^2}{8\pi G}R_h^3,
\qquad v=HR_h\sqrt{\Delta_c/2}.
$$

The supplied expansion law gives $H(3)=286.49\,\mathrm{km\,s^{-1}Mpc^{-1}}$, and hence $R_h=v/(10H)=97.74\,\mathrm{kpc}$. Taking $\kappa=1$ yields

$$
\boxed{R_d\simeq9.77\,\mathrm{kpc},\qquad v_d\simeq280\,\mathrm{km\,s^{-1}}.}
$$

The corresponding [virial mass of a dark-matter halo](../../../../../virial-mass-of-a-dark-matter-halo.md) is $M_h\simeq1.78\times10^{12}M_\odot$, and $M_d\simeq1.78\times10^{11}M_\odot$. Other overdensity conventions give $R_d\propto\Delta_c^{-1/2}$ at fixed $H,v,\kappa$.

Interpret the wavelength separation as an observed-frame local mean near the redshift in question. Since [Lyman-alpha absorption](../../../../../lyman-alpha-absorption.md) appears at $\lambda_{\rm obs}=\lambda_\alpha(1+z)$, the incidence is

$$
\frac{dN_{\rm abs}}{dz}\simeq\frac{\lambda_\alpha}{\Delta\lambda_{\rm obs}}=2.
$$

Assume one counted absorption system per intercepted disk, no unrelated forest systems or missed absorbers, unity neutral covering fraction, and a locally slowly varying population. Let $\sigma_{\rm abs}$ be the proper interception cross-section and $n_c$ the [comoving number density](../../../../../comoving-number-density.md). The proper density is $n_p=n_c(1+z)^3$, and the proper line element along the light path is $dl_p=c\,dz/[H(z)(1+z)]$. Thus the [absorber incidence and comoving number density](../../../../../absorber-incidence-and-comoving-number-density.md) relation is

$$
\boxed{\frac{dN_{\rm abs}}{dz}=n_c\sigma_{\rm abs}\frac{c(1+z)^2}{H(z)}.}
$$

For a thin circular disk, the projected area is $\pi R_d^2|\cos i|$. Isotropically oriented normals have $\langle|\cos i|\rangle=1/2$, so the [random-orientation absorbing-disk cross-section](../../../../../random-orientation-absorbing-disk-cross-section.md) is $\sigma_{\rm abs}=\pi R_d^2/2$. Consequently

$$
\boxed{n_c\simeq0.796\,\mathrm{Mpc}^{-3}\quad\text{for random orientations, }\kappa=1,\ \Delta_c=200.}
$$

If all disks are taken face-on instead, $n_c\simeq0.398\,\mathrm{Mpc}^{-3}$. Generally the random-orientation result scales as $\kappa^2(\Delta_c/200)$ and is divided by the neutral covering fraction. The finite mean redshift spacing is sizable, so a precision inference would integrate the incidence over the actual redshift interval rather than identify it with one local value.

There is also a [halo abundance mass-budget bound](../../../../../halo-abundance-mass-budget-bound.md) on this formal result. The present mean matter density for these parameters is $\bar\rho_{m,0}=\Omega_m3H_0^2/(8\pi G)\simeq3.40\times10^{10}M_\odot\,\mathrm{Mpc}^{-3}$. Distinct haloes of this mass cannot have $n_cM_h>\bar\rho_{m,0}$, even if every matter particle belonged to them. Yet the inferred random-orientation population has

$$
\frac{n_cM_h}{\bar\rho_{m,0}}\simeq42,\qquad
 n_{c,\max}=\frac{\bar\rho_{m,0}}{M_h}\simeq0.019\,\mathrm{Mpc}^{-3}.
$$

Even the face-on estimate exceeds this bound by about twenty-one. **The numerical incidence result is conditional; the supplied population assumptions are not cosmologically consistent under this standard virial and compact-disk estimate.** A larger neutral-gas absorption radius, a different absorber population, or different physical inputs are needed. For example, random orientations would require an absorbing radius at least about $63\,\mathrm{kpc}$ merely to reach the all-matter upper bound, much larger than the calculated centrifugal radius. This check does not change the algebraic answer, but prevents treating it as a realizable population.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
