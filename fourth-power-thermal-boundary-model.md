# Fourth-power thermal boundary model

↑ **Parent:** [Kapitza resistance](kapitza-resistance.md)

Choose a positive constant $\Sigma$ and the illustrative interface law

$$
q=\Sigma(T_h^4-T_c^4),\qquad
[\Sigma]=\mathrm{W\,m^{-2}\,K^{-4}},\qquad T_h\geq T_c>0.
$$

Here $T_h$ and $T_c$ are the hot and cold interface-side [temperatures](temperature-split.md), not distant [thermometer](thermometer.md) readings. This is a low-[temperature](temperature-split.md) [phonon](phonon.md) model under restrictive assumptions, not a universal fit to Kapitza's measured exponent or a material-property table. Its coefficient $\Sigma$ is not the [Stefan-Boltzmann constant](stefan-boltzmann-constant.md): the carriers in this model are [phonons](phonon.md), rather than [photons](photon.md) crossing a vacuum.

The fourth power has a simple counting explanation. In the three-dimensional low-[temperature](temperature-split.md) [Debye model](debye-model.md), a linear [phonon dispersion relation](phonon-dispersion-relation.md) gives a [density of states](density-of-states.md) proportional to $\omega^2$. A [phonon](phonon.md) has [energy](energy-split.md) $\hbar\omega$ and [Bose-Einstein distribution](bose-einstein-distribution.md) occupation $[\exp(\hbar\omega/k_BT)-1]^{-1}$. If propagation speeds and the angle-averaged transmission introduce no additional frequency scale over the occupied modes, the outgoing [energy](energy-split.md) flux has the form

$$
J(T)\propto\int_0^\infty\frac{\omega^3\,d\omega}{e^{\hbar\omega/(k_BT)}-1}
=\left(\frac{k_BT}{\hbar}\right)^4\int_0^\infty\frac{x^3\,dx}{e^x-1}\propto T^4.
$$

Extending the upper integration limit assumes occupied modes lie well below the cutoff. Balancing the two outgoing fluxes, with coefficients satisfying zero net [heat flux](heat-flux-density.md) at equal [temperatures](temperature-split.md), gives the chosen difference of fourth powers. Frequency-dependent transmission, different excitations or additional transport channels can change this conclusion.

The finite-drop area-specific [thermal resistance](thermal-resistance.md) follows by factoring a difference of powers:

$$
r_{K,\rm sec}=\frac{T_h-T_c}{q}
=\frac{1}{\Sigma(T_h+T_c)(T_h^2+T_c^2)}.
$$

Near [thermal equilibrium](thermal-equilibrium-split.md), write $T_h=T+\delta T$ and $T_c=T$. Expansion gives $q=4\Sigma T^3\delta T+O((\delta T)^2)$, so the differential area-specific [Kapitza resistance](kapitza-resistance.md) is

$$
R_K(T)=\lim_{\delta T\to0}\frac{\delta T}{q(T+\delta T,T)}
=\frac{1}{4\Sigma T^3}\quad[\mathrm{K\,m^2\,W^{-1}}],\qquad
\mathcal R_K(T)=\frac{R_K(T)}{A}\quad[\mathrm{K\,W^{-1}}].
$$

At a finite bias, varying only the hot side gives $(\partial q/\partial T_h)^{-1}=1/(4\Sigma T_h^3)$; this is generally different from $r_{K,\rm sec}$. Stating what is held fixed makes a differential resistance reproducible.

<a id="kapitza-fourth-power-boundary-model"></a>
![](kapitza-fourth-power-boundary-model.png)

**[Figure 10](#kapitza-fourth-power-boundary-model). A chosen fourth-power thermal boundary model and its differential Kapitza resistance**. [Source](kapitza-fourth-power-boundary-model.py). Original dimensionless calculations. The left curve fixes $T_c=T_0$ and compares exact [heat flux](heat-flux-density.md) with its equilibrium tangent. The right curve varies the common equilibrium [temperature](temperature-split.md) used to define $R_K$. Neither panel contains experimental measurements or fitted [helium](helium.md) properties.

For an original normalized example, choose reference scales $T_0>0$ and $A_0>0$, and set

$$
\theta_h=\frac{T_h}{T_0}=1.2,\qquad \theta_c=\frac{T_c}{T_0}=1,\qquad
j=\frac{q}{\Sigma T_0^4}=1.2^4-1=1.0736.
$$

For contact [area](surface-area.md) $A=2A_0$, the total [heat transfer](heat-transfer.md) rate is $\dot Q=2.1472A_0\Sigma T_0^4$. The finite-drop resistance satisfies $\Sigma T_0^3r_{K,\rm sec}=0.2/1.0736=125/671\approx0.18629$. Using the equilibrium tangent at $T_0$ instead would predict $j=4(0.2)=0.8$, illustrating why a substantial [temperature](temperature-split.md) rise requires the nonlinear law. Doubling the common equilibrium [temperature](temperature-split.md) reduces $R_K$ by eight in this chosen model.

A series check can be done without guessing any material properties. Stipulate a hot-side slab with dimensionless areal bulk resistance $b_s=\Sigma T_0^3L_s/k_s=0.10$, and neglect the cold-side bulk drop. At the same $j=1.0736$, the hot reservoir must have $T_H/T_0=1.2+b_sj=1.30736$. The imposed reservoir drop splits into $0.10736$ in the bulk and $0.20$ at the interface. Applying the fourth-power law directly to $T_H$ would assign the bulk drop to the interface and overestimate the [heat flux](heat-flux-density.md).

Finally, transfer [heat](heat-split.md) at rate $Aq$ between maintained interface-side [temperatures](temperature-split.md) $T_h>T_c>0$. The hot side loses [entropy](entropy-split.md) at rate $Aq/T_h$, and the cold side gains it at rate $Aq/T_c$. With no interface [entropy](entropy-split.md) accumulation, the [entropy production](entropy-production.md) per unit [area](surface-area.md) is

$$
\frac{\dot S_{\rm prod}}{A}=q\left(\frac1{T_c}-\frac1{T_h}\right)
=\Sigma\frac{(T_h-T_c)^2(T_h+T_c)(T_h^2+T_c^2)}{T_hT_c}>0.
$$

For the normalized example it is $\dot S_{\rm prod}/(A\Sigma T_0^3)=1.0736(1-1/1.2)=0.178933\ldots$. The same [energy](energy-split.md) crosses both sides in a [steady state](steady-state.md), while total [entropy](entropy-split.md) increases, consistently with the [Second law of thermodynamics](second-law-of-thermodynamics-split.md). A finite [temperature](temperature-split.md) jump during [heat transfer](heat-transfer.md) therefore expresses dissipation, not a failure of [energy](energy-split.md) conservation.

## ↑ Ancestors (9)

1. [Kapitza resistance](kapitza-resistance.md)
2. [Thermal boundary resistance](thermal-boundary-resistance.md)
3. [Cryogenics](cryogenics.md)
4. [Temperature](temperature-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Fourth-power thermal boundary model](fourth-power-thermal-boundary-model.md)
- [Kapitza resistance](kapitza-resistance.md)
