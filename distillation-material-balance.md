# Distillation material balance

↑ **Parent:** [Distillation](distillation.md)

Consider a nonreacting two-component [mixture](mixture-split.md) processed into just two products, with no losses or unaccounted inventory. Let $F,D,B$ be feed, distillate, and bottoms [amount of substance](amount-of-substance.md) values in [moles](mole-unit.md), and let $z,x_D,x_B$ be their component-A [mole fractions](mole-fraction.md). These are whole-stream compositions; $x_D$ is not automatically the instantaneous equilibrium [vapor](vapor.md) composition $y$ above the pot. Total and component balances give

$$
F=D+B,\qquad Fz=Dx_D+Bx_B.
$$

The component-B balance follows by subtracting the second equation from the first. Eliminating $B$ gives, for $x_D\ne x_B$,

$$
\frac DF=\frac{z-x_B}{x_D-x_B},\qquad
\frac BF=\frac{x_D-z}{x_D-x_B}.
$$

Nonnegative product amounts require $z$ between $x_B$ and $x_D$. For an original stipulated feed $F=1\,\mathrm{mol}$, $z=0.35$, $x_D=0.80$, and $x_B=0.10$,

$$
D=\frac5{14}\,\mathrm{mol},\qquad B=\frac9{14}\,\mathrm{mol}.
$$

Check the component inventories:

$$
Dx_D=\frac27\,\mathrm{mol},\qquad Bx_B=\frac9{140}\,\mathrm{mol},\qquad
\frac27+\frac9{140}=\frac7{20}=0.35.
$$

The distillate contains a fraction $(Dx_D)/(Fz)=40/49\approx0.816327$ of the original component A, despite its higher [mole fraction](mole-fraction.md) $x_D=0.80$. This distinction between composition and recovery is useful when deciding how much enriched product to collect. These balances determine neither [temperatures](temperature-split.md), [heat](heat-split.md) input, nor the number of [equilibrium stages](equilibrium-stage.md); they do not prove that the specified products are attainable in a particular [fractionating column](fractionating-column.md).

## ↑ Ancestors (3)

1. [Distillation](distillation.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Distillation](distillation.md)
- [Laboratory condenser](laboratory-condenser.md)
- [Repeated ideal-stage enrichment](repeated-ideal-stage-enrichment.md)
