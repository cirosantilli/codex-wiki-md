<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

In vacuum, with possible sources $\rho$ and $\mathbf J$, [Maxwell's equations](../../../maxwell-equations-split.md) are

$$
\nabla\cdot\mathbf E=\rho/\epsilon_0,\quad\nabla\cdot\mathbf B=0,\quad\nabla\times\mathbf E=-\partial_t\mathbf B,\quad\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

Their integral forms, with compatible orientations and fixed surfaces, are

$$
\begin{aligned}
\oint_{\partial V}\mathbf E\cdot d\mathbf S&=\frac1{\epsilon_0}\int_V\rho\,dV,&\quad\oint_{\partial V}\mathbf B\cdot d\mathbf S&=0,\\
\oint_{\partial S}\mathbf E\cdot d\mathbf l&=-\frac d{dt}\int_S\mathbf B\cdot d\mathbf S,&\quad\oint_{\partial S}\mathbf B\cdot d\mathbf l&=\mu_0\int_S\mathbf J\cdot d\mathbf S+\mu_0\epsilon_0\frac d{dt}\int_S\mathbf E\cdot d\mathbf S.
\end{aligned}
$$

Charge- and current-free space additionally sets $\rho=0$, $\mathbf J=0$. Vacuum constitutive constants alone do not imply that no charges exist.

Take the [curl](../../../curl.md) of the source-free [Ampere-Maxwell law](../../../ampere-s-circuital-law.md), use [Faraday's law of induction](../../../faraday-s-law-of-induction.md) and $\nabla\cdot\mathbf B=0$:

$$
\nabla\times(\nabla\times\mathbf B)=-\nabla^2\mathbf B=-\mu_0\epsilon_0\partial_t^2\mathbf B.
$$

Consequently

$$
\boxed{\nabla^2\mathbf B-\frac1{c^2}\partial_t^2\mathbf B=0,\qquad c=\frac1{\sqrt{\mu_0\epsilon_0}}.}
$$

For the specified complex [plane wave](../../../plane-wave.md), the [wavevector](../../../wavevector.md) is $k\hat{\mathbf z}$ and $\omega=ck$. [Faraday's law of induction](../../../faraday-s-law-of-induction.md) fixes

$$
\boxed{\mathbf B=\frac{E_0}{c}e^{i(\omega t-kz)}\hat{\mathbf y}.}
$$

The physical fields are the real parts. They are in phase and their [Poynting vector](../../../poynting-vector.md) points along $+z$.

The instantaneous electric and magnetic [energy densities](../../../energy-density.md) are $u_E=\epsilon_0E^2/2$ and $u_B=B^2/(2\mu_0)$. Since $E=cB$, they are equal for this ideal travelling plane wave, and so are their cycle averages: **$\langle u_E\rangle/\langle u_B\rangle=1$**. For real peak amplitude $E_0$, each average is $\epsilon_0E_0^2/4$. The [Poynting vector](../../../poynting-vector.md) and mean intensity satisfy

$$
\mathbf S=\frac1{\mu_0}\mathbf E\times\mathbf B,\qquad\boxed{\mathcal I=\langle S\rangle=\frac12\epsilon_0cE_0^2,\quad B_0=E_0/c.}
$$

It represents transported energy per area per time, in $\mathrm{W\,m^{-2}}$.

For the numerical moonlight estimate, adopt $L_\odot=3.828\times10^{26}\,\mathrm W$ and lunar mean radius $R_M=1.7374\times10^6\,\mathrm m$. These additional astronomical inputs give solar irradiance at the Moon of $\mathcal I_\odot=L_\odot/(4\pi d_\odot^2)\simeq1361\,\mathrm{W\,m^{-2}}$.[Bulk parameters: luminosity 382.8 in units of 10^24 J/s](../../../sun-fact-sheet-by-national-aeronautics-and-space-administration.md)[Bulk parameters: volumetric mean radius 1737.4 km and solar irradiance 1361 W/m^2](../../../moon-fact-sheet-by-national-aeronautics-and-space-administration.md)

Under the simple isotropic point-reflector approximation, the intercepted power is $\pi R_M^2\mathcal I_\odot$, of which fraction $A=0.12$ is redistributed over $4\pi$ steradians. Thus

$$
\mathcal I_M=\frac{A\mathcal I_\odot R_M^2}{4d_M^2}\simeq8.34\times10^{-4}\,\mathrm{W\,m^{-2}},\qquad\boxed{E_0\simeq0.793\,\mathrm{V\,m^{-1}},\quad B_0\simeq2.65\,\mathrm{nT}.}
$$

These are equivalent sinusoidal peak amplitudes; the corresponding [root mean square](../../../root-mean-square.md) fields are smaller by $\sqrt2$. Actual moonlight is broadband and incoherent.

A total reflected fraction alone does not specify the directional brightness of a full Moon. For a [Lambertian sphere at full phase](../../../lambertian-sphere-at-full-phase.md), with the same total reflectance $A$, integrating its radiance gives $\mathcal I_M=(2A/3)\mathcal I_\odot(R_M/d_M)^2$, instead giving $E_0\simeq1.30\,\mathrm{V\,m^{-1}}$ and $B_0\simeq4.32\,\mathrm{nT}$. If 0.12 is instead the [geometric albedo](../../../geometric-albedo.md), the full-phase formula is $\mathcal I_M=0.12\mathcal I_\odot(R_M/d_M)^2$, giving $E_0\simeq1.59\,\mathrm{V\,m^{-1}}$. NASA's table itself distinguishes [Bond albedo](../../../bond-albedo.md) from [geometric albedo](../../../geometric-albedo.md).[Bulk parameters list Bond albedo 0.11 and geometric albedo 0.12](../../../moon-fact-sheet-by-national-aeronautics-and-space-administration.md) The numerical estimate therefore needs an explicit reflection convention; the first boxed values use the stated isotropic approximation.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2016 resit](../../2016-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
