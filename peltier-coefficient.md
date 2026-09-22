# Peltier coefficient

↑ **Parent:** [Peltier effect](peltier-effect.md)

At uniform [temperature](temperature-split.md), define the material [Peltier coefficient](peltier-coefficient.md) by transported [heat current](heat-current.md) along positive [conventional current](conventional-current.md):

$$
\dot Q_{\rm tr}=\Pi I.
$$

Its units are $\mathrm{W/A}=\mathrm{J/C}=\mathrm V$. In one dimension, $q=\Pi j-\kappa\,dT/dx$, with [electric current density](current-density.md) $j$ and [thermal conductivity](thermal-conductivity.md) $\kappa$. Here [heat](heat-split.md) excludes the [electrochemical potential](electrochemical-potential.md) contribution to total [energy flux](energy-flux.md).[A.11.1; A.11.4, Eq. (A.34): heat-flux convention](thermoelectric-effects-by-leon-van-dommelen.md)

Now orient positive [conventional current](conventional-current.md) $I$ from material A into material B, at a common junction [temperature](temperature-split.md) $T$. Define $\dot Q_{\rm abs}>0$ as [heat](heat-split.md) taken from the junction's thermal surroundings. The outgoing transported [heat](heat-split.md) minus the incoming transported [heat](heat-split.md) gives

$$
\Pi_{A\to B}^{\rm abs}=\Pi_B-\Pi_A,\qquad
\dot Q_{\rm abs}=(\Pi_B-\Pi_A)I.
$$

The local released [heat](heat-split.md) is $\dot Q_{\rm rel}=-\dot Q_{\rm abs}$. Authors defining a junction coefficient by released [heat](heat-split.md) therefore use the opposite sign. Exchanging A and B reverses the coefficient; reversing $I$ at fixed A and B reverses the junction's thermal response. An individual material coefficient and a junction difference are different quantities.

For an original stipulated example, choose $S_A=-100\,\mu\mathrm{V/K}$ and $S_B=+150\,\mu\mathrm{V/K}$ at $T=300\,\mathrm K$. The [Kelvin thermoelectric relation](kelvin-thermoelectric-relation.md) gives $\Pi_A=-0.030\,\mathrm V$, $\Pi_B=+0.045\,\mathrm V$. A positive $2\,\mathrm A$ flowing A to B absorbs $(0.075\,\mathrm V)(2\,\mathrm A)=0.150\,\mathrm W$. A separate $0.010\,\Omega$ junction [electrical resistance](electrical-resistance.md) would dissipate $0.040\,\mathrm W$ for either direction. If all that dissipation heats the junction, its net absorbed [power](power.md) is $0.110\,\mathrm W$ forwards and $-0.190\,\mathrm W$ backwards. These numbers illustrate a chosen thermal accounting boundary, not measured material data or a universal allocation of contact heating.

**Table of contents**

- [Kelvin thermoelectric relation](kelvin-thermoelectric-relation.md)

## ↑ Ancestors (6)

1. [Peltier effect](peltier-effect.md)
2. [Thermoelectric effect](thermoelectric-effect-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Kelvin thermoelectric relation](kelvin-thermoelectric-relation.md)
- [Peltier coefficient](peltier-coefficient.md)
- [Peltier effect](peltier-effect.md)
