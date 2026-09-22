# Local Joule heating rate

↑ **Parent:** [Joule heating](joule-heating.md)

The [electric field](electric-field.md) does [work](work.md) on matter at local [power](power.md) per [volume](volume.md)

$$
p_{\rm vol}=\mathbf J\cdot\mathbf E,\qquad
[p_{\rm vol}]=\frac{\mathrm A}{\mathrm{m^2}}\frac{\mathrm V}{\mathrm m}
=\mathrm{W\,m^{-3}}.
$$

Here $\mathbf J$ is [current density](current-density.md) and the [dot product](dot-product.md) includes the relative direction. Positive $\mathbf J\cdot\mathbf E$ means [energy](energy.md) passes from the field to matter; negative means matter supplies [energy](energy.md) to the field. In general this is a [work](work.md) rate, not automatically an irreversible heating rate.[§27–2, equations 27.3–27.5 and the intervening charge-force argument: work on matter per unit volume and its sign in the field-energy balance](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

For a stationary [isotropic](isotropy.md) [Ohmic conductor](ohmic-conductor.md) with real scalar [electrical conductivity](electrical-conductivity.md) $\sigma>0$, local [Ohm's law](ohm-s-law.md) gives $\mathbf J=\sigma\mathbf E$. Thus the [local Joule heating rate](local-joule-heating-rate.md) is

$$
p_{\rm vol}=\sigma|\mathbf E|^2
=\frac{|\mathbf J|^2}{\sigma}
=\rho_{\rm el}|\mathbf J|^2\geq0,\qquad
\rho_{\rm el}=\frac1\sigma.
$$

The [electrical resistivity](electrical-resistivity.md) $\rho_{\rm el}$ has units $\Omega\,\mathrm m$, and [electrical conductivity](electrical-conductivity.md) has units $(\Omega\,\mathrm m)^{-1}$. These formulas use the material's rest frame and dissipative conduction [current density](current-density.md). Moving media, [complex conductivity](complex-conductivity.md), and additional storage or transport processes require their appropriate [energy](energy.md) balance rather than this scalar substitution.

For [uniform current in a straight homogeneous wire](uniform-current-in-a-straight-homogeneous-wire.md) of [length](length.md) $L$, [wire cross-sectional area](wire-cross-sectional-area.md) $A$ and constant [electrical conductivity](electrical-conductivity.md), $E=V/L$, $J=I/A$ and $R=L/(\sigma A)$. The [volume integral](volume-integral.md) recovers terminal [power](power.md):

$$
P=\int_{\text{wire}}\mathbf J\cdot\mathbf E\,d^3x
=\frac IA\frac VL(AL)=IV=I^2R.
$$

As a numerical check, the wire already used in [electrical resistance](electrical-resistance.md) has $L=1\,\mathrm m$, $A=10^{-6}\,\mathrm{m^2}$, $\sigma=5\times10^5\,(\Omega\,\mathrm m)^{-1}$ and $V=5\,\mathrm V$. It gives $J=2.5\times10^6\,\mathrm{A/m^2}$, $p_{\rm vol}=1.25\times10^7\,\mathrm{W/m^3}$ and $P=12.5\,\mathrm W$, agreeing with $I=2.5\,\mathrm A$ and $R=2\,\Omega$. Concentrating the same [electric current](electric-current.md) in a smaller [wire cross-sectional area](wire-cross-sectional-area.md) therefore raises the local heating rate if [electrical resistivity](electrical-resistivity.md) stays fixed.

## ↑ Ancestors (10)

1. [Joule heating](joule-heating.md)
2. [Ohm's law](ohm-s-law.md)
3. [Electrical resistance](electrical-resistance.md)
4. [Electrical resistance and conductance](electrical-resistance-and-conductance.md)
5. [Electric current](electric-current.md)
6. [Electric charge](electric-charge.md)
7. [Electromagnetism](electromagnetism-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Local Joule heating rate](local-joule-heating-rate.md)
