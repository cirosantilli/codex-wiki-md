# Fixed-x electron scattering kinematics

↑ **Parent:** [SLAC-MIT deep inelastic electron scattering experiment](slac-mit-deep-inelastic-electron-scattering-experiment.md)

Work in [natural units](natural-units.md) with $c=1$, neglect the [electron mass](electron-mass.md), and put the initial [proton](proton.md) at rest with [mass](mass.md) $M$. Let $k$ and $k'$ be the initial and final [electron](electron.md) [four-momenta](four-momentum.md), $q=k-k'$, and $Q^2=-q^2>0$. Define the laboratory [energy](energy-split.md) transfer $\nu_{\rm lab}=E-E'=P\cdot q/M$. This $\nu_{\rm lab}$ has units of [energy](energy-split.md); the invariant $P\cdot q$ has units of [energy](energy-split.md) squared. The [Bjorken scaling variable](bjorken-scaling-variable.md) and the final [hadron](hadron.md) [invariant mass](invariant-mass.md) obey

$$
Q^2=4EE'\sin^2(\theta/2),\qquad x=\frac{Q^2}{2M\nu_{\rm lab}},\qquad W^2=(P+q)^2=M^2+Q^2\left(\frac1x-1\right).
$$

These follow by squaring $k-k'$ and $P+q$, using $k^2=k'^2=0$ and $P=(M,\mathbf0)$. Solving the [Bjorken x](bjorken-x.md) definition gives the outgoing [energy](energy-split.md) and then the [scattering angle](scattering-angle.md):

$$
E'=E-\frac{Q^2}{2Mx},\qquad \sin^2\frac\theta2=\frac{Q^2}{4E(E-Q^2/(2Mx))}.
$$

Alternatively, substituting $Q^2=4EE'\sin^2(\theta/2)$ before solving gives $E'=E/[1+2E\sin^2(\theta/2)/(Mx)]$. A chosen $x,E,Q^2$ must satisfy $E'>0$ and $0\leq\sin^2(\theta/2)\leq1$. In addition, $W$ must exceed the lightest allowed inelastic [hadron](hadron.md) threshold; positive $W^2$ alone is insufficient.

For an original numerical example, take $M=0.938\,\mathrm{GeV}$, $x=0.3$, $E=15\,\mathrm{GeV}$ and $Q^2=3\,\mathrm{GeV}^2$. Then $\nu_{\rm lab}\simeq5.330\,\mathrm{GeV}$, $E'\simeq9.670\,\mathrm{GeV}$, $\theta\simeq8.25^\circ$, and $W\simeq2.807\,\mathrm{GeV}$. Varying $2\leq Q^2/\mathrm{GeV}^2\leq5$ and $10\leq E/\mathrm{GeV}\leq20$ at this same [Bjorken x](bjorken-x.md) keeps every setting physical and gives $W^2>5.54\,\mathrm{GeV}^2$, above the [proton](proton.md)-[pion](pion.md) threshold and the stricter chosen continuum selection $W>2\,\mathrm{GeV}$. These are calculated settings, not historical measurements.

## ↑ Ancestors (8)

1. [SLAC-MIT deep inelastic electron scattering experiment](slac-mit-deep-inelastic-electron-scattering-experiment.md)
2. [Deep inelastic scattering](deep-inelastic-scattering.md)
3. [Quantum chromodynamics](quantum-chromodynamics.md)
4. [Standard Model](standard-model-split.md)
5. [Quantum field theory](quantum-field-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
