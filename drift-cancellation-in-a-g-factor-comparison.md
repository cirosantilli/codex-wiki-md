# Drift cancellation in a g-factor comparison

↑ **Parent:** [Spin-orbit g-factor ratio from two P states](spin-orbit-g-factor-ratio-from-two-p-states.md)

Even a shared field does not cancel if it is sampled at different times. Write $f_A(t)=g_A C(t)$ and $f_B(t)=g_B C(t)$, where $C(t)=\mu_BB(t)/h$. As an original proposed diagnostic, bracket the $B$-state reading at $t=0$ with $A$-state readings at $t=\pm\tau$:

$$
R_{\rm bracket}=
\frac{f_B(0)}{\tfrac12[f_A(-\tau)+f_A(+\tau)]}.
$$

If $C(t)=C_0(1+bt)$, the denominator is exactly $g_A C_0$, so $R_{\rm bracket}=g_B/g_A$. A single earlier $A$ reading instead gives $R_{\rm unpaired}=(g_B/g_A)/(1-b\tau)$. For the preceding numerical model and $b\tau=0.001$, this unpaired comparison falsely gives approximately $a_e=0.00186649$; interpolation recovers $0.0012$. The sequence illustrates cancellation and is not asserted to be Kusch and Foley's exact historical timing protocol.

<a id="image-cancel-a-shared-calibration-scale-without-hiding-its-limitations"></a>
![](atomic-g-ratio-field-drift.png)

**[Figure 17](#image-cancel-a-shared-calibration-scale-without-hiding-its-limitations). Cancel a shared calibration scale without hiding its limitations**. Original calculations for [spin-orbit g-factor ratio from two P states](spin-orbit-g-factor-ratio-from-two-p-states.md) and [drift cancellation in a g-factor comparison](drift-cancellation-in-a-g-factor-comparison.md). All inputs are stipulated. The left plot shows the nonlinear inversion from a frequency ratio to a spin-to-orbital [g-factor](g-factor-physics.md) ratio. The right plot contrasts an unpaired reading with a symmetric bracket under linear field drift; the dashed curve adds chosen quadratic curvature $c\tau^2=0.0002$. No curve is a measured resonance or a historical fit.

For a curved field $C(t)=C_0(1+bt+ct^2)$, the same calculation gives

$$
R_{\rm bracket}=\frac{g_B/g_A}{1+c\tau^2}.
$$

The linear drift cancels but the curvature remains. Different fields sampled by the two beams, additive frequency offsets and incorrect atomic corrections also survive. For a small ratio error $\delta R$, direct differentiation of the inverse relation gives

$$
\delta x\simeq\frac{6}{(R+1)^2}\,\delta R,\qquad
\delta a_e\simeq\frac{3}{(R+1)^2}\,\delta R\quad(g_L=1).
$$

Repeated readings can reduce random [measurement uncertainty](measurement-uncertainty.md); agreement among genuinely different state comparisons is what tests shared [systematic errors](systematic-error.md) in their interpretation.

## ↑ Ancestors (8)

1. [Spin-orbit g-factor ratio from two P states](spin-orbit-g-factor-ratio-from-two-p-states.md)
2. [Electron magnetic moment](electron-magnetic-moment.md)
3. [Magnetic dipole moment](magnetic-dipole-moment.md)
4. [Magnetic vector potential](magnetic-vector-potential.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Drift cancellation in a g-factor comparison](drift-cancellation-in-a-g-factor-comparison.md)
