# Drude conductivity and Hall experiment

↑ **Parent:** [Drude model](drude-model.md)

A motivating laboratory realization is [The Hall Effect and Conductivity in Germanium by Rex Tayloe](the-hall-effect-and-conductivity-in-germanium-by-rex-tayloe.md). The handout specifies a germanium sample holder with [temperature](temperature.md) and [magnetic field](magnetic-field.md) control, a low-voltage supply, digital meters, and a current-reversing switch. Measure the sample dimensions, map the contacts, and establish the directions of [electric current](electric-current.md), [magnetic field](magnetic-field.md), and transverse voltage. At fixed [temperature](temperature.md) and zero [magnetic field](magnetic-field.md), sweep positive and negative [electric currents](electric-current.md) and record longitudinal [electric potential differences](electric-potential-difference.md). A straight voltage-versus-[electric current](electric-current.md) relation tests [Ohm's law](ohm-s-law.md); sample geometry converts its [slope](slope.md) to [electrical resistivity](electrical-resistivity.md). For the [Hall effect](hall-effect.md), minimize the zero-field transverse offset and measure transverse voltage at all four combinations of $\pm I$ and $\pm B$, repeating for several [electric currents](electric-current.md). The readouts test longitudinal proportionality, transverse polarity, and transverse proportionality to [electric current](electric-current.md). These are protocol instructions, not reported measurement outcomes.[pp. 1–3, Equipment, Fig. 1, and At room temperature: conductivity sweep and four polarity combinations](the-hall-effect-and-conductivity-in-germanium-by-rex-tayloe.md)

For interpreting such measurements, an ideal uniform bar of [wire cross-sectional area](wire-cross-sectional-area.md) $A$ with longitudinal sensing contacts separated by $L$ gives $\sigma=L I/(A V_L)$. [Four-terminal sensing](four-terminal-sensing.md) suppresses voltage drops in current contacts when the voltage meter draws negligible [electric current](electric-current.md); it does not fix uncertain dimensions or a nonuniform [current density](current-density.md). Reverse [electric current](electric-current.md) and use $[V_L(+I)-V_L(-I)]/2$ to reject a constant voltage offset. Keep [temperature](temperature.md) stable, allow the [current density](current-density.md) to settle, and reduce [electric current](electric-current.md) to test for [Joule heating](joule-heating.md). Those are controls for interpreting the material coefficient, rather than reasons to assume every measured curve is linear.

For the transverse measurement define $\mathbf J=J_x\widehat{\mathbf x}$, $\mathbf B=B_z\widehat{\mathbf z}$, width $w$ along $y$, and thickness $d$ along $z$. Define $V_H=V(y=-w/2)-V(y=+w/2)=E_yw$, so $J_x=I/(wd)$ gives

$$
R_H=\frac{E_y}{J_xB_z}=\frac{dV_H}{IB_z}.
$$

Extract the part odd in both [electric current](electric-current.md) and [magnetic field](magnetic-field.md) using

$$
V_H^{\mathrm{odd}}=\frac{V(+I,+B)-V(-I,+B)-V(+I,-B)+V(-I,-B)}{4}.
$$

This combination rejects a constant offset and longitudinal pickup even in [magnetic field](magnetic-field.md). It cannot reject another signal with the same two reversal symmetries. Check field polarity and magnitude independently; a sign error in the contact map changes the inferred [Hall coefficient](hall-coefficient.md).

For one [Drude model](drude-model.md) species in transverse open circuit, the steady [Lorentz force](lorentz-force.md) balance is $0=q(\mathbf E+\mathbf v_d\times\mathbf B)-m\mathbf v_d/\tau$ with $v_{d,y}=0$. Its $y$ component gives $E_y=v_{d,x}B_z$. Consequently

$$
R_H=\frac1{nq},\qquad
R_H=-\frac1{ne}\quad\text{for electrons},\qquad
n=\frac1{e|R_H|},\qquad
\mu=\sigma|R_H|=\frac{e\tau}{m},\qquad
\tau=\frac{m\sigma}{ne^2}.
$$

Longitudinal [electrical conductivity](electrical-conductivity.md) and the [Hall coefficient](hall-coefficient.md) therefore separate [number density](number-density.md) from [charge carrier mobility](charge-carrier-mobility.md) in this single-species model. Inferring a [momentum relaxation time](momentum-relaxation-time.md) additionally requires an appropriate [mass](mass.md). A constant-field longitudinal measurement alone cannot supply all three.

A [Hall coefficient](hall-coefficient.md) is not universally the reciprocal of signed [number density](number-density.md). For example, adding independent [Electron](electron.md) and [electron hole](electron-hole.md) contributions with densities $n,p$ and positive [charge carrier mobilities](charge-carrier-mobility.md) $\mu_e,\mu_h$ in the weak-[magnetic field](magnetic-field.md) limit gives

$$
\sigma=e(n\mu_e+p\mu_h),\qquad
R_H=\frac{p\mu_h^2-n\mu_e^2}{e(n\mu_e+p\mu_h)^2}.
$$

The [Hall coefficient](hall-coefficient.md) can vanish even while [electrical conductivity](electrical-conductivity.md) is positive, and its sign weights [charge carrier mobility](charge-carrier-mobility.md) as well as [number density](number-density.md). The germanium handout explicitly asks students to track possible transverse sign changes with [temperature](temperature.md); it does not establish a universal single-carrier interpretation. Real [electronic band structure](electronic-band-structure.md) and unequal scattering also limit that interpretation.[p. 1, Experiment, and p. 3, As a function of temperature: tracking carrier sign and Hall-voltage sign changes](the-hall-effect-and-conductivity-in-germanium-by-rex-tayloe.md)

## ↑ Ancestors (11)

1. [Drude model](drude-model.md)
2. [Electrical conductivity](electrical-conductivity.md)
3. [Ohm's law](ohm-s-law.md)
4. [Electrical resistance](electrical-resistance.md)
5. [Electrical resistance and conductance](electrical-resistance-and-conductance.md)
6. [Electric current](electric-current.md)
7. [Electric charge](electric-charge.md)
8. [Electromagnetism](electromagnetism-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Hall effect](hall-effect.md)
