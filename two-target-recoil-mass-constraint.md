# Two-target recoil mass constraint

↑ **Parent:** [Neutron detection by proton recoil](neutron-detection-by-proton-recoil.md)

A single recoil endpoint leaves a tradeoff between incident [speed](speed.md) and projectile [mass](mass.md). Two targets can remove the unknown incident [speed](speed.md). Assume both runs sample the same maximum projectile [speed](speed.md) $v$ and that single [elastic collisions](elastic-collision.md) reach the endpoint. For initially stationary target [masses](mass.md) $M_1<M_2$, let their maximum recoil [speeds](speed.md) be $u_1,u_2$. The [maximum elastic recoil energy fraction](maximum-elastic-recoil-energy-fraction.md) calculation gives

$$
u_i=\frac{2m}{m+M_i}v,\qquad
R=\frac{u_1}{u_2}=\frac{m+M_2}{m+M_1},\qquad
m=\frac{M_2-RM_1}{R-1}.
$$

If [energies](energy-split.md) rather than [speeds](speed.md) are inferred, use $R=\sqrt{T_{1,\max}M_2/(T_{2,\max}M_1)}$. The [energy](energy-split.md) ratio itself is not the [speed](speed.md) ratio.

For the stipulated $4\,\mathrm{MeV}$ example, [hydrogen](hydrogen.md) and [nitrogen](nitrogen.md) give

$$
\frac{M_1}{m_p}=1,\qquad \frac{M_2}{m_p}=14,\qquad
R=\sqrt{\frac{4\times14}{224/225}}=\frac{15}{2},\qquad
\frac{m}{m_p}=\frac{14-15/2}{15/2-1}=1.
$$

The inferred [mass](mass.md) then determines $v=u_1(m+M_1)/(2m)$. Changing the assumed [mass](mass.md) to improve one recoil endpoint changes the prediction for the other: this is the constraining power of the comparison.

[James Chadwick](james-chadwick.md)'s June paper instead used approximate endpoints $u_p=3.3\times10^7\,\mathrm{m/s}$ and $u_N=4.7\times10^6\,\mathrm{m/s}$, obtaining $m/m_p\simeq1.15$; it allowed roughly ten percent uncertainty in $u_N$. This was a rough [mass](mass.md) comparison.[Section 3, pages 698–699: endpoint equations and uncertainty](the-existence-of-a-neutron-by-james-chadwick.md)

The inverse calculation has useful built-in checks. A positive finite [mass](mass.md) requires $1<R<M_2/M_1$. As $R$ approaches $1$, distinguishing large projectile [masses](mass.md) becomes difficult. Differentiation gives

$$
\frac{dm}{dR}=\frac{M_1-M_2}{(R-1)^2}.
$$

Uncertain recoil endpoints therefore produce an uncertain inferred [mass](mass.md); the collision model cannot turn imprecise range measurements into exact spectroscopy. If different target runs select different incident [energy](energy-split.md) groups, the common-$v$ cancellation also fails.

For comparison, [Compton scattering](compton-scattering.md) of a [photon](photon.md) of [energy](energy-split.md) $E_\gamma$ from a stationary free target of [mass](mass.md) $M$ has the exact relativistic endpoint

$$
T_{\gamma,\max}=\frac{2E_\gamma^2}{Mc^2+2E_\gamma},\qquad
E_\gamma=\frac{T+\sqrt{T^2+2TMc^2}}{2}.
$$

This follows by combining [momentum conservation](momentum-conservation.md) with the target's relativistic [energy](energy-split.md), maximizing transfer when the [photon](photon.md) reverses direction. Unlike the massive-projectile calculation, this equation does not approximate the incident [photon](photon.md) as a [nonrelativistic particle](nonrelativistic-particle.md).

As a separate, explicitly hypothetical test, take $m_pc^2=938\,\mathrm{MeV}$ and target rest [energies](energy-split.md) $938\,\mathrm{MeV}$ and $14\times938\,\mathrm{MeV}$. To reproduce the stipulated [hydrogen](hydrogen.md) recoil endpoint $T=4\,\mathrm{MeV}$, the [photon](photon.md) would need $E_\gamma\simeq45.36\,\mathrm{MeV}$. The same [photon](photon.md) would give the heavier target at most $0.311\,\mathrm{MeV}$, whereas the stipulated massive projectile gave $0.996\,\mathrm{MeV}$. This is the structure of a two-target discrimination, not a transcription of a 1932 measurement. Actual radiation can contain more than one [energy](energy-split.md) group or both [photons](photon.md) and neutrons; a useful model must account for the observed endpoints and their origin together.

## ↑ Ancestors (8)

1. [Neutron detection by proton recoil](neutron-detection-by-proton-recoil.md)
2. [Neutron](neutron-split.md)
3. [Nucleon](nucleon.md)
4. [Baryon](baryon.md)
5. [Hadron](hadron.md)
6. [Subatomic particle](subatomic-particle.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
