# Limits of adiabatic demagnetization

↑ **Parent:** [Adiabatic demagnetization](adiabatic-demagnetization.md)

Three distinct effects spoil indefinite $T\propto B$ cooling: extra [entropy](entropy-split.md) outside the spin subsystem, additional magnetic [energy](energy-split.md) scales, and irreversible [heat](heat-split.md) or [work](work.md) input. They can be distinguished with a thermodynamic [derivative](derivative.md). For a smooth equilibrium [Helmholtz free energy](helmholtz-free-energy.md) obeying $dF=-S\,dT-m\,dB$, a [Maxwell relation](maxwell-relations.md) gives

$$
dS=\frac{C_B}{T}\,dT+\left(\frac{\partial m}{\partial T}\right)_B dB,\qquad
\left(\frac{dT}{dB}\right)_S=-\frac{T}{C_B}\left(\frac{\partial m}{\partial T}\right)_B.
$$

Here $C_B$ is the total [heat capacity](heat-capacity.md) participating in the stage's [thermal equilibrium](thermal-equilibrium-split.md). The ideal model has $(\partial m/\partial T)_B=-C_{B,{\rm mag}}/B$. If its spins share [temperature](temperature-split.md) with a field-independent lattice and load of combined [heat capacity](heat-capacity.md) $C_{\rm other}>0$, then

$$
\left(\frac{dT}{dB}\right)_{S_{\rm total}}
=\frac{T}{B}\frac{C_{B,{\rm mag}}}{C_{B,{\rm mag}}+C_{\rm other}}.
$$

The positive slope still means cooling when $dB<0$, but its smaller magnitude gives less cooling per fractional field reduction. For example, a low-[temperature](temperature-split.md) [Debye model](debye-model.md) gives a lattice [entropy](entropy-split.md) proportional to $T^3$. As that lattice [entropy](entropy-split.md) falls, the spins take up the released [entropy](entropy-split.md); $x$ can no longer remain constant. A weak enough coupling to neglect its equilibrium interaction [energy](energy-split.md) can still be strong enough to exchange [heat](heat-split.md) on the sweep timescale.

Interactions between [magnetic moments](magnetic-dipole-moment.md), including [exchange interaction](exchange-interaction.md) and the fields of neighboring [magnetic dipole moments](magnetic-dipole-moment.md), introduce [energy](energy-split.md) scales that do not vanish with the applied $B$. Once they compete with $k_BT$ or $\mu B$, the independent-site [partition function](canonical-partition-function.md) fails. Correlations and possible magnetic ordering alter the available [magnetic entropy](magnetic-entropy.md) and the cooling curve. Simply setting the external [magnetic field](magnetic-field-split.md) to zero does not eliminate those interactions. Different refrigerants therefore need their own measured equilibrium properties; there is no universal final [temperature](temperature-split.md) from the applied-field ratio alone.

Finally, a real open [heat switch](heat-switch.md) has residual [thermal conductance](thermal-conductance.md); supports, wires and radiation carry incoming [heat](heat-split.md). Field changes may also dissipate [energy](energy-split.md). Locally near [thermal equilibrium](thermal-equilibrium-split.md), with incoming [heat](heat-split.md) rate $\dot Q_{\rm leak}$ and internal [entropy production](entropy-production.md) rate $\dot S_{\rm prod}$, the stage balance becomes

$$
\frac{dS}{dt}=\frac{\dot Q_{\rm leak}}T+\dot S_{\rm prod},\qquad
C_B\dot T=-T\left(\frac{\partial m}{\partial T}\right)_B\dot B
+\dot Q_{\rm leak}+T\dot S_{\rm prod}.
$$

This uses a common stage [temperature](temperature-split.md); a non-equilibrated load requires separate balances. The sweep must allow [spin-lattice relaxation](spin-lattice-relaxation.md) while remaining fast enough to limit accumulated parasitic [heat](heat-split.md). At fixed $B$, the same balance explains warming and finite hold time. Useful refrigeration is the controlled absorption of a load's [heat](heat-split.md) during that finite interval, followed by a renewed [isothermal process](isothermal-process.md) of [magnetization](magnetization.md) to export its [entropy](entropy-split.md).

## ↑ Ancestors (7)

1. [Adiabatic demagnetization](adiabatic-demagnetization.md)
2. [Temperature](temperature-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
