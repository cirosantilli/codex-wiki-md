# Cockcroft-Walton multiplier model

↑ **Parent:** [Cockcroft-Walton generator](cockcroft-walton-generator.md)

Define a stage as one storage increment of $2V_p$, with $V_p$ the alternating input's peak [electric potential difference](electric-potential-difference.md) relative to its reference, not its peak-to-peak value. Assume ideal [rectifiers](rectifier.md), no load, no leakage or stray [capacitance](capacitance.md), a stiff alternating source and enough cycles to reach equilibrium. For $N$ such stages,

$$
V_k=2kV_p,\qquad k=0,1,\ldots,N,\qquad V_{\mathrm{ideal}}=2NV_p.
$$

The factor two follows from adding the input's next opposite excursion to an already stored peak. The subsequent series increments add. This ideal argument concerns equilibrium voltage; it supplies neither the charge-up time nor the useful load [electric current](electric-current.md).

To isolate the effect of drawing charge, consider the following original reservoir model. Each storage stage has equal [capacitance](capacitance.md) $C$; a constant output [electric current](electric-current.md) $I$ removes $\Delta q=I/f$ between replenishment events of [frequency](frequency.md) $f$. Every series reservoir loses this charge, hence its voltage falls by $a=I/(fC)$ per interval. Suppose replenishment removes a fixed fraction $1-\lambda$ of each reservoir's accumulated deficit, with $0\leq\lambda<1$. This is an explicit phenomenological pump rule, not a solution of a particular multiplier's rectifier network. If $d_j$ is the deficit immediately after event $j$, then

$$
d_{j+1}=\lambda(d_j+a),\qquad
d_+=\frac{\lambda a}{1-\lambda},\qquad
d_-=\frac{a}{1-\lambda}.
$$

Here $d_+$ and $d_-$ are the equilibrium deficits just after and just before replenishment. Linear discharge between events gives the average output and peak-to-peak variation

$$
\overline V_{\mathrm{out}}=2NV_p-N\frac{I}{fC}\frac{1+\lambda}{2(1-\lambda)},\qquad
V_{\mathrm{pp}}=N\frac{I}{fC}.
$$

For chosen dimensionless settings $N=3$, $a/V_p=0.020$ and $\lambda=1/2$, the output varies between $5.88V_p$ and $5.94V_p$, averaging $5.91V_p$, instead of the unloaded $6V_p$. Starting with zero deficit, the recurrence approaches equilibrium geometrically with factor $\lambda$. Taking $I\to0$ recovers the ideal ladder; increasing $C$ or $f$ reduces droop in this model. As $\lambda\to1$, effective replenishment fails and the small-deficit assumption fails too.

Real multiplier stages have unequal charge-transfer burdens; their mean deficits need not be equal and depend on topology, input impedance and parasitic [capacitance](capacitance.md). Thus this reservoir model explains droop and voltage variation without claiming their exact dependence on stage count for a real [Cockcroft-Walton generator](cockcroft-walton-generator.md). In particular, adding more stages cannot be judged solely by the unloaded $2NV_p$. For a beam sampling a slowly varying output, the [electrostatic acceleration energy gain](electrostatic-acceleration-energy-gain.md) follows that instantaneous potential drop, so voltage variation also produces a spread of beam [kinetic energies](kinetic-energy.md).

## ↑ Ancestors (6)

1. [Cockcroft-Walton generator](cockcroft-walton-generator.md)
2. [Electrostatic accelerator](electrostatic-accelerator.md)
3. [Particle accelerator](particle-accelerator-split.md)
4. [Experimental apparatus](experimental-apparatus.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
