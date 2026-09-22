# Strong acid titration model

↑ **Parent:** [Acid-base titration](acid-base-titration.md)

Consider an original ideal model: $V_A=10.00\,\mathrm{mL}$ of [hydrochloric acid](hydrochloric-acid.md) at $c_A=0.100\,\mathrm{mol\,L^{-1}}$, titrated with [sodium hydroxide](sodium-hydroxide.md) at $c_B=0.100\,\mathrm{mol\,L^{-1}}$. Treat these numbers as exact model inputs. Assume complete [dissociation of an ionic compound](dissociation-of-an-ionic-compound.md), complete [strong acid](strong-acid.md) ionization, additive [volumes](volume.md), uniform mixing, and [activity coefficients](activity-coefficient.md) equal to one. Use stipulated $K_w=10^{-14}$, approximately appropriate near $25\,{}^\circ\mathrm C$. These are calculated [pH](ph.md) values, not measurements of these materials.

The [chemical equation](chemical-equation.md) for [neutralization](neutralization.md) is

$$
\mathrm{H_3O^+}+\mathrm{OH^-}\longrightarrow2\mathrm{H_2O}.
$$

Initial acid inventory is $n_A=1.000\,\mathrm{mmol}$, so the [equivalence point](equivalence-point.md) is $v=10.00\,\mathrm{mL}$. Added [water](water.md) does not change this inventory. But the final [volume](volume-thermodynamics.md) $V_A+v$, including the [titrant](titrant.md), determines all [concentrations](concentration.md).

Keep [self-ionization of water](self-ionization-of-water.md) even at the [equivalence point](equivalence-point.md). With $c^\circ=1\,\mathrm{mol\,L^{-1}}$, define the [dimensionless](dimensionless-quantity.md) acid excess $d$, [hydronium](hydronium.md) level $h$, and [hydroxide](hydroxide.md) level $o$ by

$$
d=\frac{c_AV_A-c_Bv}{c^\circ(V_A+v)},\qquad h=\frac{[\mathrm{H_3O^+}]}{c^\circ},\qquad o=\frac{[\mathrm{OH^-}]}{c^\circ}.
$$

The [sodium](sodium.md) [cation](cation.md) and [chloride](chloride.md) [anion](anion.md) inventories fix the [electric charge](electric-charge-split.md) balance $h-o=d$, while [chemical equilibrium](chemical-equilibrium.md) gives $ho=K_w$. Eliminating $o$ yields a [quadratic equation](quadratic-equation.md) $h^2-dh-K_w=0$ with exactly one positive [root](root-of-a-root-system.md). For stable calculation on either side, write

$$
s=\sqrt{d^2+4K_w},\qquad
h=\begin{cases}(d+s)/2,&d\geq0,\\2K_w/(s-d),&d<0,\end{cases}
\qquad o=\frac{K_w}{h},\qquad \mathrm{pH}=-\log_{10}h.
$$

The second expression follows by multiplying by $s-d$; it avoids subtracting two nearly equal large quantities on the alkaline side. A [logarithm](logarithm.md) acts on the [dimensionless](dimensionless-quantity.md) $h$, as required by the [pH](ph.md) definition.

<a id="strong-acid-titration-water-equilibrium"></a>
![](strong-acid-titration-water-equilibrium.png)

**[Figure 2](#strong-acid-titration-water-equilibrium). An ideal strong acid titration curve stays smooth through its equivalence point because of self-ionization of water**. Original analytic model for $10.00\,\mathrm{mL}$ of $0.100\,\mathrm{mol\,L^{-1}}$ [hydrochloric acid](hydrochloric-acid.md) and $0.100\,\mathrm{mol\,L^{-1}}$ [sodium hydroxide](sodium-hydroxide.md), with $K_w=10^{-14}$. Both panels use the complete [electric charge](electric-charge-split.md) balance and ideal [chemical equilibrium](chemical-equilibrium.md). The right panel resolves microlitre additions around the [equivalence point](equivalence-point.md). The marked points are calculated, not measured.

At $v=5.00\,\mathrm{mL}$, the excess is $0.500\,\mathrm{mmol}$ in $15.00\,\mathrm{mL}$, giving $d=1/30$ and [pH](ph.md) $1.477121\ldots$. At $v=15.00\,\mathrm{mL}$, excess [hydroxide](hydroxide.md) is $0.500\,\mathrm{mmol}$ in $25.00\,\mathrm{mL}$, giving $d=-1/50$ and [pH](ph.md) $12.301030\ldots$. Neglecting [dilution](dilution.md) would give the wrong values even far from the [equivalence point](equivalence-point.md).

Exactly at $v=10.00\,\mathrm{mL}$, $d=0$ and $h=o=\sqrt{K_w}=10^{-7}$, giving [pH](ph.md) $7$ in this model. At $9.999\,\mathrm{mL}$ and $10.001\,\mathrm{mL}$, the same smooth expression gives [pH](ph.md) $5.300835\ldots$ and $8.699121\ldots$. The familiar excess-only formulas would predict zero [hydronium](hydronium.md) or zero [hydroxide](hydroxide.md) at the [equivalence point](equivalence-point.md); retaining [self-ionization of water](self-ionization-of-water.md) removes that failure. A steep curve is still continuous.

The sensitivity is especially revealing. Differentiating $h-K_w/h=d$ gives

$$
\frac{\mathrm d(\mathrm{pH})}{\mathrm d d}=-\frac{1}{\ln(10)\sqrt{d^2+4K_w}},\qquad
\left.\frac{\mathrm d d}{\mathrm d v}\right|_{v=V_A}=-\frac{c_A}{2c^\circ V_A}
$$

when $c_A=c_B$. At this model's [equivalence point](equivalence-point.md), the [derivative](derivative.md) is about $1.086\times10^4$ [pH](ph.md) units per millilitre. This is a local [derivative](derivative.md), not a linear prediction over a whole drop. Real endpoint accuracy also depends on dosing, mixing, [measurement uncertainty](measurement-uncertainty.md), [temperature](temperature-split.md), extra reacting [chemical species](chemical-species.md), and nonideal [thermodynamic activities](thermodynamic-activity.md).

## ↑ Ancestors (7)

1. [Acid-base titration](acid-base-titration.md)
2. [Weak acid dissociation measurement](weak-acid-dissociation-measurement.md)
3. [Weak acid](weak-acid.md)
4. [Acid (chemistry)](acid-chemistry.md)
5. [Acid-base chemistry](acid-base-chemistry-split.md)
6. [Chemistry](chemistry-split.md)
7. [Codex Wiki](split.md)
