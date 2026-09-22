<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $z$ upwards and write $\zeta=z+Wt$, so that the unperturbed interface is $\zeta=0$, with [carbon dioxide](../../../../../carbon-dioxide.md) above and [water](../../../../../water.md) below. Use the sharp-interface, [incompressible flow](../../../../../incompressible-flow.md) version of [Darcy's law](../../../../../darcy-law.md), with constant [porosity](../../../../../porosity.md) and [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md), no [capillary pressure](../../../../../capillary-pressure.md), and effectively unbounded layers. The distinction between [Darcy flux](../../../../../darcy-velocity.md) and interface speed matters: the base flux is $q_z=-\phi W$, since the printed $W$ is the speed of the interface. Thus the base [pressure gradients](../../../../../pressure-gradient.md) satisfy

$$
p_{j,z}^0=\frac{\mu_j\phi W}{k}-\rho_jg,\qquad j=c,w.
$$

The [mass density](../../../../../density.md) ordering is stabilizing, whereas injection of the less viscous fluid into the more viscous fluid produces the [Saffman–Taylor instability](../../../../../saffman-taylor-instability.md).

For [linear stability analysis](../../../../../linear-stability.md), displace the interface by $\eta=\widehat\eta e^{\sigma t+i\alpha x}$. Taking the [divergence](../../../../../divergence.md) of [Darcy's law](../../../../../darcy-law.md) shows that the perturbation [pressure](../../../../../pressure.md) satisfies the [Laplace equation](../../../../../laplace-equation.md). Decay away from the interface gives, for $a_\alpha=|\alpha|>0$,

$$
p'_c=Ae^{-a_\alpha\zeta}e^{\sigma t+i\alpha x},\qquad p'_w=Be^{a_\alpha\zeta}e^{\sigma t+i\alpha x}.
$$

The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) and continuity of normal [Darcy flux](../../../../../darcy-velocity.md) give

$$
\phi\sigma\widehat\eta=\frac{k a_\alpha A}{\mu_c}=-\frac{k a_\alpha B}{\mu_w}.
$$

Meanwhile [pressure continuity](../../../../../pressure-continuity.md), evaluated on the displaced interface, gives

$$
A-B=-\widehat\eta(p_{c,z}^0-p_{w,z}^0)=\widehat\eta\left[\frac{\phi W(\mu_w-\mu_c)}k-g(\rho_w-\rho_c)\right].
$$

Eliminating $A,B$ yields the [buoyancy-modified Darcy fingering dispersion relation](../../../../../buoyancy-modified-darcy-fingering-dispersion-relation.md):

$$
\boxed{\sigma(\alpha)=\frac{|\alpha|}{\phi(\mu_w+\mu_c)}\left[\phi W(\mu_w-\mu_c)-kg(\rho_w-\rho_c)\right].}
$$

Every nonzero [wavenumber](../../../../../wavenumber.md) decays when $W<W_c$, grows when $W>W_c$, and is neutral at equality, where

$$
\boxed{W_c=\frac{kg(\rho_w-\rho_c)}{\phi(\mu_w-\mu_c)}.}
$$

The zero [wavenumber](../../../../../wavenumber.md) is a uniform displacement and is neutral. Without a short-scale regularization such as [surface tension](../../../../../surface-tension.md), this model has no fastest-growing finite [wavenumber](../../../../../wavenumber.md): on the unstable side its [growth rate](../../../../../growth-rate.md) increases without bound as $|\alpha|$ increases. Finite layer depths would change the [dispersion relation](../../../../../dispersion-relation.md); none are specified here.

Taking $g=9.81\,\mathrm{m\,s^{-2}}$ and a year of $365.25$ days, the data give

$$
\phi W_c=3.27\times10^{-6}\,\mathrm{m\,s^{-1}}\simeq103.2\,\mathrm{m\,yr^{-1}},\qquad \boxed{W_c\simeq\frac{103.2}{\phi}\,\mathrm{m\,yr^{-1}}.}
$$

The numerical paragraph supplies no [porosity](../../../../../porosity.md), so it cannot determine a unique numerical interface speed. If $W$ were instead intended to mean [Darcy velocity](../../../../../darcy-velocity.md), the numerical critical value would be $103.2\,\mathrm{m\,yr^{-1}}$, and the interface would move at $W/\phi$. These two velocity conventions must not be conflated.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
