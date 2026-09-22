# Paper 349

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_349.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_349.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 349](paper-349.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

With the convention in the question, the constant [velocity-anisotropy parameter](../../../galaxy.md#velocity-anisotropy-parameter) is $\beta=1-\sigma_t^2/\sigma_r^2$. Since $V_c^2=r\,d\Phi/dr$, the [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation) becomes

$$
\frac{d(\nu\sigma_r^2)}{dr}
+\frac{2\beta}{r}\nu\sigma_r^2
=-\frac{\nu V_c^2}{r}.
$$

For $\nu=\nu_0r^{-\alpha}$ and $V_c^2=V_0^2r^{2\gamma}$, its general [integrating factor](../../../differential-equation.md#integrating-factor) solution is

$$
\boxed{\sigma_r^2(r)=
\frac{V_c^2(r)}{\alpha-2\beta-2\gamma}
+Cr^{\alpha-2\beta}.}
$$

The homogeneous term represents a boundary pressure. For an extended scale-free system the physical boundary condition normally removes it, leaving

$$
\boxed{\sigma_r^2=\frac{V_c^2}{\alpha-2\beta-2\gamma}.}
$$

Positivity requires $\alpha-2\beta-2\gamma>0$. A complete physical model must also have a nonnegative [galactic distribution function](../../../galaxy.md#galactic-distribution-function) and sensible inner and outer boundary behaviour; for example, strong radial anisotropy is restricted by density-slope--anisotropy inequalities.

Observationally, the tracer density can be estimated from star counts only after correcting distances, extinction, survey selection, and incompleteness. Spectroscopy supplies mainly line-of-sight velocities; proper motions add transverse information but become less precise for distant halo stars. The equation shows the [mass--anisotropy--density degeneracy](../../../galaxy.md#mass-anisotropy-density-degeneracy) directly: the same measured $\sigma_r$ can result from a larger $V_c$, a steeper tracer slope $\alpha$, or a different $\beta$. Even globally constant power laws therefore do not determine the galactic mass profile unless some of these quantities are independently constrained.

If $\alpha$, $\beta$, or $\gamma$ changes near a break radius, the solution at one radius also depends on the outer boundary integral. A break in observed dispersion may be attributed to a mass-profile feature, a tracer-density break, or a change in orbital anisotropy. Separate tracer populations, full three-dimensional velocities, higher velocity moments, and measurements over a wide radial range help break this degeneracy.

More flexible alternatives model a nonnegative solution of the [Collisionless Boltzmann equation](../../../galaxy.md#collisionless-boltzmann-equation) itself. An [action-based galactic distribution function](../../../galaxy.md#action-based-galactic-distribution-function) gives an analytic or parametrized $f(\mathbf J)$; a [Schwarzschild orbit-superposition model](../../../galaxy.md#schwarzschild-orbit-superposition-model) assigns nonnegative weights to an orbit library; and a [made-to-measure stellar-dynamical model](../../../galaxy.md#made-to-measure-stellar-dynamical-model) adjusts particle weights to reproduce observations. These methods retain more phase-space information than Jeans moments, although their flexibility introduces model choices and regularization.

## 2

↑ **Parent:** [Paper 349](paper-349.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Direct evidence for [stellar feedback](../../../galaxy.md#stellar-feedback) includes expanding ionized shells and superbubbles around young associations, hot X-ray-emitting gas in [supernova remnants](../../../galaxy.md#supernova-remnant), broad or split emission lines, and blueshifted absorption showing cool and warm [outflows](../../../galaxy.md#galactic-outflow). P-Cygni profiles reveal massive-star winds, while extraplanar filaments and metal-enriched gas demonstrate transport away from star-forming disks. Indirect evidence includes the galaxy mass--metallicity relation, low baryon fractions and suppressed star formation in dwarf galaxies, chemically enriched circumgalactic gas, and correlations of outflow speed and mass loading with the [star formation rate](../../../galaxy.md#star-formation-rate).

Rapid gas removal changes the gravitational potential before stellar and dark-matter orbits can respond adiabatically. Positions and velocities are initially unchanged, but orbital binding energies rise; orbits expand and become more eccentric, and some particles escape. Repeated burst--outflow--reaccretion cycles can irreversibly transfer energy to collisionless matter and turn a central dark-matter cusp into a core. This matters because dwarf-galaxy rotation curves are used to test dark-matter microphysics: a feedback-made core can mimic a non-cold or self-interacting dark-matter signature.

Write the initial potential energy as $W=-aGM^2/R$. The [virial theorem](../../../classical-mechanics.md#virial-theorem) gives $T=-W/2$. If a well-mixed fraction $\epsilon$ remains after instantaneous mass loss, the immediate kinetic and potential energies are $T_a=\epsilon T$ and $W_a=\epsilon^2W$, so

$$
E_a=T_a+W_a
=a\frac{GM^2}{R}\left(\frac\epsilon2-\epsilon^2\right).
$$

After revirialization at $R'$, $E_f=W_f/2=-aG\epsilon^2M^2/(2R')$. Equating energies gives the [impulsive mass-loss expansion law](../../../galaxy.md#impulsive-mass-loss-expansion-law)

$$
\boxed{\frac{R'}R=\frac{\epsilon}{2\epsilon-1}.}
$$

The remnant is bound only for $\epsilon>1/2$; loss of half or more of the gravitating mass disrupts this idealized system.

For many infinitesimal, individually revirialized losses, put $\epsilon=1+dM/M$ in the impulsive result. To first order, $dR/R=-dM/M$. Integration yields the [adiabatic mass-loss expansion law](../../../galaxy.md#adiabatic-mass-loss-expansion-law)

$$
\boxed{MR=\text{constant},\qquad \frac{R'}R=\frac1\epsilon.}
$$

Slow loss causes finite expansion for every positive remaining mass fraction and has no sharp disruption threshold.

Finally consider an initially circular orbit of radius $R$ around a point mass $M$. Its speed and specific angular momentum obey $v^2=GM/R$ and $h^2=GMR$. Immediately after $M\to\epsilon M$, these remain unchanged, while the new specific energy is

$$
E'=\frac{GM}{R}\left(\frac12-\epsilon\right).
$$

Using the [orbital eccentricity](../../../classical-mechanics.md#orbital-eccentricity) relation $e^2=1+2E'h^2/(G^2\epsilon^2M^2)$ gives

$$
\boxed{e=\frac{1-\epsilon}{\epsilon}.}
$$

It is an ellipse for $\epsilon>1/2$, parabolic at $\epsilon=1/2$, and unbound for smaller $\epsilon$, in agreement with the virial argument.

## 3

↑ **Parent:** [Paper 349](paper-349.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Kennicutt–Schmidt law](../../../stellar-astrophysics.md#kennicutt-schmidt-law) is the empirical relation

$$
\Sigma_{\rm SFR}=A\Sigma_g^N,
\qquad N\simeq1.4
$$

for disk-averaged total gas, with a nearly linear molecular-gas relation in many resolved observations. Atomic gas is mapped through the H I 21-cm line, molecular gas mainly through carbon-monoxide line emission and a CO-to-$\mathrm H_2$ conversion factor, and star formation through combinations of ultraviolet continuum, H-alpha recombination emission, and infrared dust emission. Inclination, dust attenuation, the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function), tracer lifetimes, and conversion factors must be treated consistently.

The gas-depletion time $M_g/\dot M_*$ is typically of order a gigayear, whereas a giant molecular cloud has a dynamical or free-fall time of order a few megayears. Star formation is therefore inefficient per collapse time, commonly at the percent level, rather than converting an entire cloud in one free fall.

For the first [closed-box model of galactic chemical evolution](../../../galaxy.md#closed-box-model-of-galactic-chemical-evolution), neglect returned mass or absorb it into the definitions. Then

$$
\frac{dM_g}{dt}=-\dot M_*=-\frac{M_g}{\tau_*},
$$

and hence

$$
\boxed{M_g=M_{g0}e^{-t/\tau_*},
\qquad \dot M_*=\frac{M_{g0}}{\tau_*}e^{-t/\tau_*},
\qquad Z=y_Z\log\frac{M_{g0}}{M_g}=\frac{y_Zt}{\tau_*}.}
$$

Thus a region reaching $Z_\odot=0.014$ after an enrichment time $t_\odot$ with $y_Z=0.006$ has

$$
\boxed{\tau_*=\frac{y_Z}{Z_\odot}t_\odot\simeq0.43t_\odot,}
$$

about $4.3\,\mathrm{Gyr}$ for a fiducial $t_\odot\simeq10\,\mathrm{Gyr}$ enrichment age of the Galactic disk.

The second prescription implies $\dot M_*=M_g^2/(M_{g0}\widetilde\tau_*)$. Solving the gas-consumption equation gives

$$
\boxed{M_g=\frac{M_{g0}}{1+t/\widetilde\tau_*},
\qquad
\dot M_*=\frac{M_{g0}}{\widetilde\tau_*}
\left(1+\frac{t}{\widetilde\tau_*}\right)^{-2},
\qquad
Z=y_Z\log\left(1+\frac{t}{\widetilde\tau_*}\right).}
$$

Therefore

$$
\boxed{\widetilde\tau_*
=\frac{t_\odot}{e^{Z_\odot/y_Z}-1}
\simeq0.107t_\odot\simeq1.1\,\mathrm{Gyr}.}
$$

For long-lived stars, $dN$ is proportional to $dM_*=-dM_g$. In the exponential model,

$$
\frac{dN}{dZ}\propto
\dot M_*\frac{dt}{dZ}
=\frac{M_{g0}}{y_Z}e^{-Z/y_Z}.
$$

In the second model, $1+t/\widetilde\tau_*=e^{Z/y_Z}$; multiplying its star-formation rate by $dt/dZ$ gives exactly the same result:

$$
\boxed{\frac{dN}{dZ}\propto e^{-Z/y_Z}.}
$$

The metallicity distribution is fixed by the closed-box relation $M_g/M_{g0}=e^{-Z/y_Z}$ and is independent of the star-formation history. Merely changing the time law therefore does not cure the [G-dwarf problem](../../../galaxy.md#g-dwarf-problem); gas inflow, outflow, variable yields, or selection effects must alter the closed-box assumptions.

## 4

↑ **Parent:** [Paper 349](paper-349.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A star-forming galaxy contains short-lived, massive O and B stars whose hot photospheres dominate the ultraviolet and blue continuum and ionize surrounding gas. Once star formation ceases, these stars disappear quickly and an older, cooler stellar population produces a redder spectrum with stronger stellar absorption features and a prominent 4000-angstrom break.

In star-forming regions, direct stellar continuum is accompanied by nebular free-bound and free-free continuum, hydrogen and helium recombination lines, collisionally excited metal lines, and infrared emission from dust that absorbed shorter-wavelength photons. Supernova remnants and cosmic rays add synchrotron radio emission, while hot shocked gas can emit X-rays.

The [Strömgren sphere](../../../galaxy.md#stromgren-sphere) model assumes a steady ionizing source in uniform, static, pure hydrogen of number density $n_H$, with a sharp [ionization front](../../../galaxy.md#ionization-front) enclosing fully ionized gas. If $N_i=(4\pi/3)R^3n_H$ is the number of ions, photon conservation gives

$$
\frac{dN_i}{dt}=\dot N_{\rm ion}
-\frac{4\pi}{3}R^3\alpha n_H^2.
$$

The equilibrium [Strömgren radius](../../../galaxy.md#stromgren-radius) and [recombination time](../../../galaxy.md#recombination-time) are

$$
R_S^3=\frac{3\dot N_{\rm ion}}{4\pi\alpha n_H^2},
\qquad t_{\rm rec}=\frac1{\alpha n_H}.
$$

Consequently the radius obeys

$$
3R^2\frac{dR}{dt}
=\frac{R_S^3-R^3}{t_{\rm rec}}.
$$

Writing $x=(R/R_S)^3$ turns this into $dx/d(t/t_{\rm rec})=1-x$. For an initially neutral medium, $x(0)=0$, and the [Ionization-front growth of a Strömgren sphere](../../../galaxy.md#ionization-front-growth-of-a-stromgren-sphere) is

$$
\boxed{R(t)=R_S\left(1-e^{-t/t_{\rm rec}}\right)^{1/3}.}
$$

The front initially expands rapidly because few ions are recombining and asymptotically approaches $R_S$ as recombinations balance ionizations. This photon-counting solution precedes any pressure-driven hydrodynamic expansion of the H II region.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
