# Conductometric saponification assay

↑ **Parent:** [Second-order reaction](second-order-reaction.md)

How can an invisible change in [concentration](concentration.md) produce a readable signal? The [saponification](saponification.md) of [ethyl acetate](ethyl-acetate.md) by [hydroxide](hydroxide.md) in [water](water.md) gives [ethanol](ethanol.md) and an [acetate ion](acetate-ion.md):

$$
\mathrm{CH_3COOC_2H_5}+\mathrm{OH^-}\longrightarrow\mathrm{CH_3COO^-}+\mathrm{C_2H_5OH}.
$$

The [rate law](rate-law.md) used for this assay is $r=k_2[\mathrm{ethyl\ acetate}][\mathrm{OH^-}]$. Each [reactant](reactant.md) has coefficient one, so $r$ equals either [disappearance rate](disappearance-rate.md). If the two initial [concentrations](concentration.md) are equal, they remain equal under this [stoichiometry](stoichiometry.md), giving $-dc/dt=k_2c^2$ and $k_{\mathrm{obs}}=k_2$, without a factor of two.

[Manual for Advanced Physical Chemistry Laboratory-II by Nasima Arshad](manual-for-advanced-physical-chemistry-laboratory-ii-by-nasima-arshad.md) (Unit 7, Experiment 2, printed pp. 66–67) specifies a conductivity cell holding about $60\,\mathrm{mL}$ in constant-[temperature](temperature-split.md) baths, with $0.040\,\mathrm{mol\,L^{-1}}$ [ethyl acetate](ethyl-acetate.md) and [sodium hydroxide](sodium-hydroxide.md) stocks equilibrated separately. Mixing $30\,\mathrm{mL}$ of each initiates the run. The readout is [electrical resistance](electrical-resistance.md): every minute for ten minutes, every two minutes for ten more, then every five minutes for twenty-five. The cell is rinsed with distilled [water](water.md). A matched [sodium hydroxide](sodium-hydroxide.md)–[water](water.md) dilution estimates the initial resistance; a [potassium chloride](potassium-chloride.md) standard determines the cell constant. The manual asks for comparison with the extrapolated initial signal.[Unit 7, Experiment 2, printed pp. 66–67: Procedure and Calculations; title page credits Nasima Arshad as manual author](manual-for-advanced-physical-chemistry-laboratory-ii-by-nasima-arshad.md)

The post-mixing initial [concentration](concentration.md) is $c_0=0.040(30/60)=0.020\,\mathrm{mol\,L^{-1}}$ for each [reactant](reactant.md), assuming additive [volumes](volume.md). This matches our illustrative starting [concentration](concentration.md), but the prescribed $k_{\mathrm{obs}}=0.50$ is not a measured value from the manual. As [hydroxide](hydroxide.md) is replaced by the less mobile [acetate ion](acetate-ion.md), [electrical conductance](electrical-conductance.md) decreases. The preceding experiment describes two [platinum](platinum.md) [electrodes](electrode.md) and an alternating-voltage [Wheatstone bridge](wheatstone-bridge.md) to limit polarization at the [electrodes](electrode.md). For measured [electrical resistance](electrical-resistance.md) $R(t)$, [electrical conductance](electrical-conductance.md) is $G(t)=1/R(t)$; [electrical conductivity](electrical-conductivity.md) is $\kappa(t)=K_{\mathrm{cell}}G(t)$. Keep the probe geometry fixed and use one signal convention throughout.[Unit 7, Experiment 1, printed pp. 62–63: reaction, ionic conductances, inverse resistance, platinum electrodes and alternating-voltage bridge; Experiment 2, p. 66: hydroxide replaced by acetate](manual-for-advanced-physical-chemistry-laboratory-ii-by-nasima-arshad.md)

For the equal-starting-[concentration](concentration.md) model, assume an affine calibration between [electrical conductance](electrical-conductance.md) and remaining [hydroxide](hydroxide.md) [concentration](concentration.md), with endpoints $G_0$ and $G_\infty$ at the same [temperature](temperature-split.md). This gives

$$
\frac{c(t)}{c_0}=\frac{G(t)-G_\infty}{G_0-G_\infty},\qquad
\frac{G_0-G(t)}{G(t)-G_\infty}=\frac{c_0-c(t)}{c(t)}=k_2c_0t.
$$

The last plot has slope $k_2c_0$, with units $\mathrm{s^{-1}}$, whereas plotting $1/c$ against time has slope $k_2$, with units $\mathrm{L\,mol^{-1}\,s^{-1}}$. These are different slopes. This endpoint transformation also shows why raw resistance must not be substituted for conductance.

Useful additional controls are repeat runs, fixed immersion depth, an independently checked final signal, and comparisons of several starting [concentrations](concentration.md). Mixing delay obscures early conversion; [temperature](temperature-split.md) drift changes both the [rate constant](rate-constant.md) and the signal; contamination adds mobile [ions](ion.md). The affine calibration can fail when ionic mobilities change with composition. Near completion, $G-G_\infty$ becomes small, so endpoint error is strongly amplified. Those are methodological limits and proposed checks, not new experimental observations. A conductivity trace supports a calibrated [rate law](rate-law.md) over its tested range; it does not independently reveal the full [reaction mechanism](reaction-mechanism.md).

For unequal starting [concentrations](concentration.md) $a=[\mathrm A]_0$ and $b=[\mathrm B]_0$ in a one-to-one [chemical reaction](chemical-reaction-split.md), let $x$ be the consumed [concentration](concentration.md). Then $[\mathrm A]=a-x$, $[\mathrm B]=b-x$, and

$$
\frac{dx}{dt}=k_2(a-x)(b-x),\qquad
\frac1{b-a}\ln\!\left(\frac{a(b-x)}{b(a-x)}\right)=k_2t\quad(a\ne b).
$$

The [natural logarithm](natural-logarithm.md) acts on a [dimensionless quantity](dimensionless-quantity.md); differentiating the left side with respect to $x$ gives $1/((a-x)(b-x))$, verifying the relation. Mixing $20\,\mathrm{mL}$ of the stated [ethyl acetate](ethyl-acetate.md) stock with $40\,\mathrm{mL}$ of the [sodium hydroxide](sodium-hydroxide.md) stock would give $a=0.01333\ldots$ and $b=0.02666\ldots\,\mathrm{mol\,L^{-1}}$. The difference $[\mathrm B]-[\mathrm A]=b-a$ stays constant, rather than their ratio. Neither the equal-[concentration](concentration.md) reciprocal formula nor a [pseudo-first-order reaction](pseudo-first-order-reaction.md) approximation is justified solely by that twofold excess.

## ↑ Ancestors (8)

1. [Second-order reaction](second-order-reaction.md)
2. [Order of reaction](order-of-reaction.md)
3. [Rate law](rate-law.md)
4. [Reaction rate](reaction-rate.md)
5. [Chemical kinetics](chemical-kinetics-split.md)
6. [Chemical reaction](chemical-reaction-split.md)
7. [Chemistry](chemistry-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Acetate ion](acetate-ion.md)
- [Ethyl acetate](ethyl-acetate.md)
- [Saponification](saponification.md)
