# Buffer capacity

↑ **Parent:** [Buffer solution](buffer-solution.md)

[Buffer capacity](buffer-capacity.md) measures resistance to a change in [pH](ph.md): how much additional [chemical acid](acid-chemistry.md) or [chemical base](base-chemistry.md) a [chemical solution](solution-chemistry.md) accommodates per small change in [pH](ph.md). Its differential form is a local [derivative](derivative.md), rather than the total inventory available before a [buffer solution](buffer-solution.md) is exhausted. Two [buffer solutions](buffer-solution.md) can have identical [pH](ph.md) and very different [buffer capacities](buffer-capacity.md).

Choose a constant [volume](volume-thermodynamics.md) $V$ and fixed [temperature](temperature-split.md). Let $n_B$ count added [moles](mole-unit.md) of fully dissociated, monovalent [chemical base](base-chemistry.md) supplying [hydroxide](hydroxide.md), and $n_A$ added [moles](mole-unit.md) of fully dissociated, monovalent [strong acid](strong-acid.md) supplying [hydrogen ions](hydrogen-ion.md). Neither addition supplies the [weak acid](weak-acid.md) component itself. The signed addition is $b=(n_B-n_A)/V$, with units $\mathrm{mol\,L^{-1}}$, and

$$
\beta=\frac{\mathrm db}{\mathrm d\mathrm{pH}}=\frac1V\frac{\mathrm dn_B}{\mathrm d\mathrm{pH}}=-\frac1V\frac{\mathrm dn_A}{\mathrm d\mathrm{pH}}.
$$

The last two forms describe separate base-only and acid-only additions. The [buffer capacity](buffer-capacity.md) is positive for the stable [chemical equilibrium](chemical-equilibrium.md) model below and is reported in $\mathrm{mol\,L^{-1}}$ per unit of [pH](ph.md). Since [pH](ph.md) is [dimensionless](dimensionless-quantity.md), the dimensional unit is just $\mathrm{mol\,L^{-1}}$; stating “per [pH](ph.md)” makes the measurement convention clear. Here constant [volume](volume-thermodynamics.md) is an idealization, realized approximately by small additions of concentrated reagent.

For a sufficiently small addition, $\Delta\mathrm{pH}\approx\Delta b/\beta$. A large [buffer capacity](buffer-capacity.md) means a small local change of [pH](ph.md) for a given addition. Over a finite interval, use the changing [buffer capacity](buffer-capacity.md) instead:

$$
\Delta b=\int_{\mathrm{pH}_0}^{\mathrm{pH}_1}\beta(p)\,\mathrm dp.
$$

This [integral](integral-split.md) gives a finite dose in $\mathrm{mol\,L^{-1}}$; it need not equal the initial [buffer capacity](buffer-capacity.md) times the eventual change in [pH](ph.md).

**Table of contents**

- [Buffer capacity of a monoprotic acid](buffer-capacity-of-a-monoprotic-acid.md)
- [Buffer capacity and concentration](buffer-capacity-and-concentration.md)
- [Finite titrant response of a buffer](finite-titrant-response-of-a-buffer.md)
- [Buffer capacity measurement](buffer-capacity-measurement.md)

## ↑ Ancestors (4)

1. [Buffer solution](buffer-solution.md)
2. [Acid-base chemistry](acid-base-chemistry-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Buffer capacity](buffer-capacity.md)
- [Buffer capacity and concentration](buffer-capacity-and-concentration.md)
- [Buffer capacity measurement](buffer-capacity-measurement.md)
- [Buffer capacity of a monoprotic acid](buffer-capacity-of-a-monoprotic-acid.md)
- [Buffer solution](buffer-solution.md)
- [Finite titrant response of a buffer](finite-titrant-response-of-a-buffer.md)
- [Henderson-Hasselbalch equation](henderson-hasselbalch-equation.md)
