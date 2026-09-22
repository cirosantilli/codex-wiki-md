# Paper 347

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_347.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_347.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $u=-v_r>0$ denote the inward speed. Steady spherical [mass conservation](../../../continuum-mechanics.md#mass-conservation) and the radial [momentum equation](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) for an [isothermal gas](../../../astrophysics.md#isothermal-bondi-accretion) give

$$
\dot M=4\pi r^2\rho u,
\qquad
u\frac{du}{dr}=-c_s^2\frac{d\log\rho}{dr}-\frac{GM}{r^2}.
$$

Eliminating $d\log\rho/dr$ produces the [Isothermal Bondi equation](../../../astrophysics.md#isothermal-bondi-equation)

$$
\left(u-\frac{c_s^2}{u}\right)\frac{du}{dr}
=\frac{2c_s^2}{r}-\frac{GM}{r^2}.
$$

A smooth flow can cross [Mach number](../../../compressible-flow.md#mach-number) one only where both sides vanish. Its [Bondi sonic point](../../../astrophysics.md#bondi-sonic-point) is therefore

$$
u_s=c_s,
\qquad
r_s=\frac{GM}{2c_s^2}.
$$

The integrated [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) which approaches rest and density $\rho_\infty$ at infinity is

$$
\frac{u^2}{2}+c_s^2\log\frac{\rho}{\rho_\infty}-\frac{GM}{r}=0.
$$

At the [sonic point](../../../compressible-flow.md#sonic-point) this gives $\rho_s=e^{3/2}\rho_\infty$, and hence the unique regular [transonic branch](../../../compressible-flow.md#transonic-branch) has

$$
\boxed{\dot M
=4\pi r_s^2\rho_s c_s
=\pi e^{3/2}\frac{G^2M^2\rho_\infty}{c_{s,\infty}^3}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

This mode is most plausible for a nearly stationary [supermassive black hole](../../../astrophysics.md#supermassive-black-hole) immersed in the hot, pressure-supported, X-ray-emitting atmosphere of a massive elliptical galaxy. Such gas is comparatively smooth, its random and rotational speeds can be smaller than its [sound speed](../../../compressible-flow.md#speed-of-sound), and radiative cooling can be slow on the inflow scale.

The ideal [Bondi accretion](../../../astrophysics.md#bondi-accretion) assumptions can fail in several independent ways. The gas may carry enough [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) to circularize into an [accretion disk](../../../astrophysics.md#accretion-disk); a galaxy's stars and dark matter can dominate the gravitational potential outside the black hole's sphere of influence; the hole can move relative to the gas; cooling, conduction, or external heating can destroy adiabaticity or isothermality; a multiphase or clumpy medium is not a uniform reservoir; magnetic fields, turbulence, and viscosity add stresses absent from the spherical model; and [AGN feedback](../../../astrophysics.md#active-galactic-nucleus-feedback), winds, or jets can expel or recirculate the inflow. Time dependence and self-gravity provide further failures. Thus a Bondi estimate is best interpreted as an idealized supply rate, not automatically as the rate crossing the event horizon.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

If $c_{s,\infty}\gg\sigma$ and $M_{\rm enc}\to M$, expansion of the denominator gives

$$
\boxed{\dot M\simeq
\pi\frac{G^2M^2\rho_\infty}{c_{s,\infty}^3},}
$$

the stated model's pressure-dominated [Bondi accretion](../../../astrophysics.md#bondi-accretion) limit. Its order-unity coefficient differs from the $\pi e^{3/2}$ found for the exactly isothermal critical solution because such coefficients depend on the adopted equation of state and interpolation.

If instead $\sigma\gg c_{s,\infty}$,

$$
\boxed{\dot M\simeq
\pi\frac{G^2M_{\rm enc}^2\rho_\infty}{\sigma^3}.}
$$

The gas's thermal motion is then negligible beside the galactic [velocity dispersion](../../../galaxy.md#velocity-dispersion), and the enclosed galactic mass, rather than the black hole alone, focuses the gas. For a [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere), $M_{\rm enc}(R)=2\sigma^2R/G$, so this becomes $\dot M\simeq4\pi\rho_\infty\sigma R^2$. This second limit describes capture controlled by the host potential and is therefore not a genuinely spherical black-hole Bondi solution.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $w=1/r$ and $h=r^2\dot\theta=bv_\infty$. Since $\dot r=-h\,dw/d\theta$, the radial equation becomes the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\frac{d^2w}{d\theta^2}+w=\frac{GM}{h^2},
$$

whose solution is

$$
w=c_1\cos\theta+c_2\sin\theta+\frac{GM}{b^2v_\infty^2}.
$$

Choose the incoming asymptote at $\theta=\pi$ and the downstream axis at $\theta=0$. Then $w\to0$ as $\theta\to\pi$, while $r\sin\theta\to b$. These two conditions give

$$
c_1=\frac{GM}{b^2v_\infty^2},
\qquad c_2=\frac1b.
$$

The mirror-image streamlines meet on the downstream axis at

$$
\boxed{r_{\rm coll}=\frac{b^2v_\infty^2}{2GM}.}
$$

At that point each streamline has radial velocity $-v_\infty$ and equal and opposite azimuthal velocity. An inelastic collision cancels the latter, so the specific energy afterwards is

$$
E_{\rm after}=\frac{v_\infty^2}{2}-\frac{GM}{r_{\rm coll}}
=\frac{v_\infty^2}{2}-\frac{2G^2M^2}{b^2v_\infty^2}.
$$

The gas is bound when $E_{\rm after}<0$, or

$$
\boxed{b<b_{\rm crit}=\frac{2GM}{v_\infty^2}.}
$$

Sweeping the corresponding capture cylinder through gas of density $\rho_\infty$ gives the [Bondi--Hoyle--Lyttleton accretion rate](../../../astrophysics.md#bondi-hoyle-lyttleton-accretion-rate)

$$
\boxed{\dot M=\pi b_{\rm crit}^2\rho_\infty v_\infty
=\frac{4\pi G^2M^2\rho_\infty}{v_\infty^3}.}
$$

Unlike stationary spherical [Bondi accretion](../../../astrophysics.md#bondi-accretion), this is a directed, supersonic flow with a downstream focusing wake; bulk speed replaces sound speed as the main resistance to capture.

## 2

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An optically thick annulus radiates as a [blackbody](../../../astrophysics.md#blackbody) from both faces, so

$$
2\sigma_{\rm SB}T_{\rm BB}^4=F_{\rm diss}.
$$

For a steady [Keplerian accretion disk](../../../astrophysics.md#keplerian-accretion-disk) with a [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition),

$$
\nu\Sigma=\frac{\dot M}{3\pi}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right],
\qquad
R^2\left(\frac{d\Omega}{dR}\right)^2=\frac94\Omega_K^2.
$$

Consequently

$$
F_{\rm diss}=\frac{3GM\dot M}{4\pi R^3}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]
$$

and

$$
\boxed{T_{\rm BB}(R)=
\left\{\frac{3GM\dot M}{8\pi\sigma_{\rm SB}R^3}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]\right\}^{1/4}.}
$$

Away from the inner edge, $T\propto R^{-3/4}$.

Ignoring inclination and distance factors, the [multitemperature blackbody disk](../../../astrophysics.md#multitemperature-blackbody-disk) spectrum is

$$
S_{\bar\nu}\propto\int_{R_{\rm in}}^{R_{\rm out}}
2\pi R B_{\bar\nu}[T(R)]\,dR.
$$

Set $x=h\bar\nu/(k_BT)$. Since $T\propto R^{-3/4}$, $R\,dR\propto\bar\nu^{-8/3}x^{5/3}dx$, whereas the [Planck function](../../../astrophysics.md#planck-function) contributes $\bar\nu^3/(e^x-1)$. In the stated intermediate-frequency range the radial endpoints become $0$ and $\infty$, leaving a frequency-independent convergent integral. Therefore

$$
\boxed{S_{\bar\nu}\propto\bar\nu^{1/3}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The standard [Shakura--Sunyaev thin disk](../../../astrophysics.md#shakura-sunyaev-thin-disk) has three qualitative radial zones. Its hot inner part is dominated by [radiation pressure](../../../thermodynamics.md#radiation-pressure) and [electron-scattering opacity](../../../stellar-structure.md#electron-scattering-opacity); farther out, [gas pressure](../../../thermodynamics.md#gas-pressure) overtakes radiation pressure while electron scattering can remain the main opacity; in the cool outer zone, gas pressure remains dominant and [free-free opacity](../../../stellar-structure.md#free-free-opacity) becomes important. The transition radii vary with $M$, $\dot M$, and $\alpha$.

For the inner zone, hold the [surface density](../../../astrophysics.md#surface-density-of-a-disk) $\Sigma$ fixed during a local thermal perturbation. Vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives

$$
P_{\rm rad}\sim\Sigma\Omega_K^2H,
\qquad P_{\rm rad}\propto T_c^4,
$$

so $H\propto T_c^4/\Sigma$. The [alpha disk](../../../astrophysics.md#alpha-disk) prescription then yields

$$
Q^+\sim\nu\Sigma\Omega_K^2
\sim\alpha\Sigma\Omega_K^3H^2
\propto\frac{T_c^8}{\Sigma},
$$

whereas optically thick radiative diffusion with nearly constant electron-scattering opacity gives

$$
Q^-\propto\frac{T_c^4}{\kappa_{\rm es}\Sigma}.
$$

At equilibrium $Q^+=Q^-=Q_0$. For net cooling $\dot Q=Q^--Q^+$,

$$
\left.\frac{\partial\dot Q}{\partial T_c}\right|_\Sigma
=\frac{4Q_0}{T_c}-\frac{8Q_0}{T_c}
=-\frac{4Q_0}{T_c}<0.
$$

Thus the total-pressure alpha prescription predicts [thermal instability of a radiation-pressure-dominated alpha disk](../../../astrophysics.md#thermal-instability-of-a-radiation-pressure-dominated-alpha-disk): a temperature increase makes heating outrun cooling. The absence of ubiquitous, large-amplitude thermal limit cycles in luminous [AGN](../../../astrophysics.md#active-galactic-nucleus) light curves indicates that this local model omits stabilizing effects, plausibly magnetic pressure and stress, vertical advection, winds, or a stress law that does not simply track total pressure.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Steady [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $\dot M=-2\pi R\Sigma u_R$. Substituting this into the angular-momentum equation and integrating from the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit) with zero torque gives

$$
\nu\Sigma R^3\frac{d\Omega}{dR}
=-\frac{\dot M}{2\pi}(l-l_{\rm ISCO})
=R\Sigma u_R(l-l_{\rm ISCO}).
$$

Therefore

$$
u_R=\frac{\nu R^2\,d\Omega/dR}{l-l_{\rm ISCO}}.
$$

Using $\nu=\alpha c_sH$, $c_s\simeq H\Omega$, $l=Ru_\phi$, and $R\,d\Omega/dR$ of order $-\Omega$ gives

$$
\boxed{|u_R|\simeq
\alpha\frac{H^2}{R^2}
\frac{u_\phi l}{l-l_{\rm ISCO}},}
$$

up to the order-unity Keplerian factor $3/2$.

At the sonic transition, $|u_R|\simeq c_s\simeq(H/R)u_\phi$. Hence

$$
\frac{l-l_{\rm ISCO}}l\simeq\alpha\frac HR\ll1
$$

for a geometrically thin disk with $\alpha\ll1$. The [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) therefore differs only fractionally from $l_{\rm ISCO}$ before the gas enters the [plunging region of a black-hole accretion disk](../../../astrophysics.md#plunging-region-of-a-black-hole-accretion-disk). Its much shorter inflow time then prevents appreciable viscous transport, justifying angular-momentum conservation across the ISCO and the zero-torque boundary condition.

## 3

↑ **Parent:** [Paper 347](paper-347.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [maximal radiative efficiency of black-hole accretion](../../../astrophysics.md#maximal-radiative-efficiency-of-black-hole-accretion) is the fraction of rest-mass energy available if all binding energy released before capture escapes as radiation. In a Newtonian disk ending at $R_{\rm in}$,

$$
\eta_{\max}=\frac{GM}{2R_{\rm in}c^2},
$$

because a circular orbit has specific binding energy $GM/(2R)$. In relativity, $\eta_{\max}=1-E_{\rm ISCO}$. Black-hole spin moves the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit) inward for prograde flow and outward for retrograde flow, increasing or decreasing this maximum respectively.

Since $L=\eta\dot M c^2$, a source of fixed luminosity requires $\dot M=L/(\eta c^2)$, while black-hole mass grows at approximately $(1-\eta)\dot M$. The actual [radiative efficiency of black-hole accretion](../../../astrophysics.md#radiative-efficiency-of-black-hole-accretion) can lie below the maximum when energy is advected through the horizon or carried away mechanically. A low-density, optically thin [advection-dominated accretion flow](../../../astrophysics.md#advection-dominated-accretion-flow) stores dissipated energy in ions, while a high-rate [slim accretion disk](../../../astrophysics.md#slim-accretion-disk) traps photons and advects their energy inward; both are [radiatively inefficient flows](../../../astrophysics.md#radiatively-inefficient-accretion-flow).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For an adiabatic [Bondi accretion](../../../astrophysics.md#bondi-accretion) flow, $\dot M\propto M^2\rho_\infty c_{s,\infty}^{-3}$. Inside the Bondi radius the speed and ion temperature are approximately virial, so $v\propto(M/r)^{1/2}$ and $T\propto M/r$, while [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $n\propto\dot M M^{-1/2}r^{-3/2}$. The frequency-integrated [thermal bremsstrahlung](../../../astrophysics.md#thermal-bremsstrahlung) emissivity is proportional to $n^2T^{1/2}$. Its volume integral is dominated by the inner flow and consequently scales as

$$
L\propto\frac{\dot M^2}{M}.
$$

Since the [Eddington luminosity](../../../stellar-structure.md#eddington-luminosity) is proportional to $M$, this may be written $L/L_{\rm Edd}=C(\dot Mc^2/L_{\rm Edd})^2$. With the standard fully ionized-plasma constants and the Bondi profiles, $\sqrt C=9\times10^{-3}$. Eliminating $\dot M$ from $\eta=L/(\dot Mc^2)$ then gives

$$
\boxed{\eta=9\times10^{-3}
\left(\frac{L}{L_{\rm Edd}}\right)^{1/2}.}
$$

The cancellation of $M$, $\rho_\infty$, and $c_{s,\infty}$ expresses the scale-free character of the ideal flow. More physically, two-body emission scales as density squared, so an increasingly dilute flow radiates a progressively smaller fraction of its available accretion power.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Soltan argument](../../../astrophysics.md#soltan-argument) compares the time-integrated luminosity density of the cosmological [AGN](../../../astrophysics.md#active-galactic-nucleus) population with the present comoving mass density in dormant [supermassive black holes](../../../astrophysics.md#supermassive-black-hole). If $U_{\rm AGN}$ is the emitted energy density corrected for obscuration and bolometric output, accretion with population-averaged efficiency $\bar\eta$ predicts

$$
\rho_{\rm BH}c^2
=\frac{1-\bar\eta}{\bar\eta}U_{\rm AGN},
\qquad
\bar\eta=\frac{U_{\rm AGN}}{U_{\rm AGN}+\rho_{\rm BH}c^2}.
$$

In practice $U_{\rm AGN}$ comes from integrating AGN [luminosity functions](../../../astrophysics.md#luminosity-function-astronomy) over luminosity and [cosmological redshift](../../../cosmology.md#cosmological-redshift), with corrections for obscured sources and missed wavebands, while $\rho_{\rm BH}$ is inferred from local galaxy--black-hole scaling relations.

The inferred efficiency is of order the canonical thin-disk value, about ten per cent, so most cosmic black-hole mass was accumulated in radiatively efficient, optically thick accretion episodes. [Radiatively inefficient flows](../../../astrophysics.md#radiatively-inefficient-accretion-flow) can dominate low-luminosity activity or brief extreme phases, and mergers redistribute existing mass, but neither naturally accounts for the observed integrated AGN radiation while supplying most of the final mass.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For a steady axisymmetric disk,

$$
\dot M=4\pi RHm_pn|u_R|,
$$

where factors of order unity depend on the vertical density profile. In a geometrically thick [advection-dominated accretion flow](../../../astrophysics.md#advection-dominated-accretion-flow), $H\sim R$, $c_s\sim v_K$, and the [alpha disk](../../../astrophysics.md#alpha-disk) estimate gives $|u_R|\sim\alpha v_K$. Thus the [inflow time](../../../astrophysics.md#inflow-time) is $t_{\rm in}\sim R/(\alpha v_K)$ and

$$
n\sim\frac{\dot M}{4\pi R^2m_p\alpha v_K}.
$$

Substitution into the given [electron--proton thermal equilibration time](../../../astrophysics.md#electron-proton-thermal-equilibration-time) yields

$$
\frac{t_{e-p}}{t_{\rm in}}
\simeq
\frac{0.24\pi\alpha^2GMm_p^2}{\dot M\sigma_Tcm_e}
\left(\frac{k_BT_e}{m_ec^2}\right)^{3/2}.
$$

Using $\dot M_{\rm Edd}=10L_{\rm Edd}/c^2=40\pi GMm_p/(\sigma_Tc)$ and a mildly relativistic electron temperature $k_BT_e/(m_ec^2)\simeq0.1$ gives

$$
\boxed{\frac{\dot M}{\dot M_{\rm Edd}}\lesssim0.4\alpha^2.}
$$

Below this rate, [Coulomb collisions](../../../statistical-physics.md#coulomb-collision) cannot transfer the ions' viscously generated heat to radiating electrons before inflow. The resulting [two-temperature accretion flow](../../../astrophysics.md#two-temperature-accretion-flow) advects most of that energy through the horizon, so its efficiency is well below the canonical $\eta\simeq0.1$ of a thin alpha disk and decreases with accretion rate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
