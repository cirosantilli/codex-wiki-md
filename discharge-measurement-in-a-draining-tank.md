# Discharge measurement in a draining tank

↑ **Parent:** [Torricelli's law](torricelli-s-law.md)

[James F. Price](james-f-price.md)'s Draining a Tank, an appendix to Dimensional Analysis of Models and Data Sets, describes an actual tabletop experiment in sections 2.1–2.3. Tap [water](water.md) filled a semitransparent polypropylene beaker with a marked [volume](volume.md) scale and drilled side openings. Some trials added horizontal outlet tubes. [Temperature](temperature-split.md) was measured, and dye checked that the [water](water.md) had settled before uncovering the outlet. The readout was elapsed time at successive [volume](volume.md) marks. Opening diameter and tube length varied between trials. Reported repeatability was checked; tube bores were measured with feeler gauges rather than accepted from nominal sizes.[James F. Price, Draining a Tank, §§2.1–2.3, printed pp. 9–12: preparation, volume/time readout and repeatability](draining-a-tank-by-james-f-price.md)

For tank [area](surface-area.md) $A$ and [volume](volume.md) $W_o$ at outlet level, the observations give $h_i=(W_i-W_o)/A$ and interval [volumetric flow rate](volumetric-flow-rate.md) $Q_i\simeq(W_i-W_{i+1})/(t_{i+1}-t_i)$. Price compared $Q/(a\sqrt{2gh})$ across heads to infer a [discharge coefficient](discharge-coefficient.md) where that ratio was nearly constant. At small head, drainage could stop with a protruding [water](water.md) cap; [surface tension](surface-tension-split.md) mattered. Outlet tubes introduced [viscosity](dynamic-viscosity-split.md) effects. This experiment tests a useful operating range, rather than proving ideal drainage down to zero head.[James F. Price, Draining a Tank, eqs. (1)–(2), Fig. 2, §3.1 eq. (13), §§4 and 5: coefficient inference and departures from ideal flow](draining-a-tank-by-james-f-price.md)

A useful independent test of the constant-coefficient model avoids numerical [derivatives](derivative.md) of noisy head readings. Its exact [square root](square-root.md) relation predicts

$$
\sqrt{h(t)}=\sqrt H-bt,\qquad
b=\frac{C_da}{A}\sqrt{\frac g2},\qquad
C_d=\frac{A}{a}\sqrt{\frac2g}\,b.
$$

Fit a straight line to $\sqrt{h_i}$ against time over a chosen positive-head interval; the negative slope determines $b$. Repeat from the same initial head and compare slopes, then vary the head interval to test constancy of $C_d$. This is a proposed diagnostic derived from the [draining tank with constant cross-sectional area](draining-tank-with-constant-cross-sectional-area.md), not an additional procedure or measured fit attributed to Price. Startup transients, uncertain outlet level, a changing jet shape and terminal low-head data can spoil the straight line. Independent collection of discharged [volume](volume.md) provides a check on the tank-scale readout.

## ↑ Ancestors (5)

1. [Torricelli's law](torricelli-s-law.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
