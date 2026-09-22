<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**[Potential temperature](../../../potential-temperature.md) and a parcel.** For a dry [ideal gas](../../../ideal-gas-split.md) of fixed composition, the [first law of thermodynamics](../../../first-law-of-thermodynamics-split.md) per unit mass is

$$
\delta q=c_p\,dT-\frac{dp}{\rho}=c_p\,dT-R_dT\frac{dp}p.
$$

A reversible [adiabatic process](../../../adiabatic-process.md) has $\delta q=0$. Taking $c_p,R_d$ constant gives $d\ln T=\kappa\,d\ln p$, where $\kappa=R_d/c_p$. Integrating to a fixed reference pressure $p_0$ defines the [potential temperature](../../../potential-temperature.md)

$$
\boxed{\Theta=T(p_0/p)^\kappa,\qquad D\Theta/Dt=0\quad\text{for dry adiabatic motion}}.
$$

It is the temperature a parcel would have after reversible dry [adiabatic process](../../../adiabatic-process.md) taking it to $p_0$. Equivalently $ds=c_p\,d\ln\Theta$ under these assumptions, making [potential temperature](../../../potential-temperature.md) a [thermodynamic entropy](../../../entropy-split.md) label useful for diagnosing stratification and air-mass motion. Latent heating, radiation, mixing and variable composition require modifying the conservation statement.

An [air parcel](../../../air-parcel.md) is a small material volume followed with the flow. The parcel model treats it as internally approximately uniform, large compared with molecular scales and small compared with environmental variation scales. Rapid [acoustic wave](../../../acoustic-wave.md) adjustment makes its pressure approximately equal to the surrounding pressure, while slower heat and mass exchange can be neglected during an idealized displacement. It is not a rigid container or an isolated molecule.

At the parcel's height, environmental hydrostatic pressure supplies an upward pressure force $\rho_e g$ per unit volume. Dividing by parcel density gives the upward acceleration

$$
B=g\left(\frac{\rho_e}{\rho_p}-1\right)=g\left(\frac{T_p}{T_e}-1\right)
=\boxed{g\frac{\Theta_p-\Theta_e}{\Theta_e}}.
$$

The last steps use equal pressure, equal gas constants and the same reference pressure. Moisture-dependent density requires virtual temperature or its potential-temperature counterpart. Nonhydrostatic pressure perturbations and [entrainment](../../../fluid-entrainment.md) are excluded from this elementary [buoyancy](../../../buoyancy.md) expression.

The [convective available potential energy](../../../convective-available-potential-energy.md) is the positive [buoyancy](../../../buoyancy.md) work per unit mass between the level of free convection and the equilibrium level:

$$
\boxed{\mathrm{CAPE}=\int_{z_{\rm LFC}}^{z_{\rm EL}}B(z)\,dz
=g\int_{z_{\rm LFC}}^{z_{\rm EL}}\frac{\Theta_p-\Theta_e}{\Theta_e}\,dz}.
$$

One sums positive-buoyancy layers when there is more than one. Negative work below free convection contributes convective inhibition rather than positive [CAPE](../../../convective-available-potential-energy.md). In a lossless parcel estimate, conversion of [CAPE](../../../convective-available-potential-energy.md) to vertical [kinetic energy](../../../kinetic-energy.md) gives $w_{\max}\simeq\sqrt{2\,\mathrm{CAPE}}$; pressure work beyond this model, mixing and precipitation can change that speed.

**[Linear stability](../../../linear-stability.md).** Let $\xi$ denote displacement from a neutrally buoyant reference altitude. Dry motion through an [adiabatic process](../../../adiabatic-process.md) retains $\Theta_p=\Theta_e(0)$, while $\Theta_e(\xi)=\Theta_e(0)+\xi\Theta_e'(0)+O(\xi^2)$. The linear vertical momentum equation is therefore

$$
\boxed{\ddot\xi+N_0^2\xi=0,\qquad N_0^2=\frac g{\Theta_e}\frac{d\Theta_e}{dz}}.
$$

For $N_0^2>0$, $\xi=C\cos N_0t+D\sin N_0t$: stable [buoyancy](../../../buoyancy.md) oscillations with period $2\pi/N_0$. For $N_0^2=0$, $\xi=C+Dt$: neutral stratification with no restoring force. For $N_0^2<0$, growing and decaying exponentials occur, indicating convective instability. The growing solution is generic unless the initial data select only the decaying branch. These are local small-displacement results with an approximately constant environmental gradient.

**Lapse-rate estimate.** Define $\Gamma=-dT/dz$. [Hydrostatic balance](../../../hydrostatic-balance.md) and the [ideal gas law](../../../ideal-gas-law.md) imply $p'/p=-g/(R_dT)$, so

$$
\boxed{\frac1\Theta\frac{d\Theta}{dz}=\frac1T\frac{dT}{dz}-\kappa\frac1p\frac{dp}{dz}
=\frac{\Gamma_d-\Gamma}{T},\qquad \Gamma_d=g/c_p}.
$$

In the free-parcel-oscillator interpretation, identifying the ridge encounter interval with the [buoyancy](../../../buoyancy.md) period gives $P=10^4/20=500\ \mathrm s$ and $N_0=2\pi/P=0.01257\ \mathrm{s^{-1}}$. With $T=293.15\ \mathrm K$, $g=9.81\ \mathrm{m\,s^{-2}}$ and $c_p\simeq1004\ \mathrm{J\,kg^{-1}\,K^{-1}}$,

$$
\boxed{\Gamma=\Gamma_d-\frac{TN_0^2}{g}\simeq5.1\ \mathrm{K\,km^{-1}}}.
$$

The frequency identification is an extra modeling assumption. A stationary mountain [gravity wave](../../../gravity-wave-split.md) generally obeys $\widehat\omega^2=N_0^2k_h^2/(k_h^2+m_z^2)$ without rotation, with $\widehat\omega=Uk_h$. Ridge spacing fixes $\widehat\omega$, not the vertical [wavenumber](../../../wavenumber.md) $m_z$. For example, $m_z=k_h$ allows the same spacing and wind with $N_0=\sqrt2\widehat\omega$, and a [lapse rate](../../../lapse-rate-atmosphere.md) about $0.3\ \mathrm{K\,km^{-1}}$. Thus $5.1$ is the requested parcel-period estimate, not a uniquely identifiable [lapse rate](../../../lapse-rate-atmosphere.md) for every possible mountain-wave field; a resolved wave field needs its vertical structure as well.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../split.md)
4. [Physics of atmospheres and oceans course of the University of Oxford](../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
