# Repeated-bath dialysis model

↑ **Parent:** [Dialysis (biochemistry)](dialysis-biochemistry.md)

Consider an original ideal model with sample [volume](volume-thermodynamics.md) $V_s$, bath [volume](volume-thermodynamics.md) $V_b$, and initial sample [solute](solute.md) [concentration](concentration.md) $c_0$. Assume each [volume](volume-thermodynamics.md) is fixed, a freely permeant, nonbinding [solute](solute.md), no [chemical reactions](chemical-reaction-split.md), complete mixing on each side, and equal [concentrations](concentration.md) at equilibrium. Each fresh bath initially contains none of this [solute](solute.md). The [protein](protein-split.md) is perfectly retained in this model.

The first equilibration redistributes the initial [amount of substance](amount-of-substance.md) $c_0V_s$ through both compartments. Conservation gives

$$
c_0V_s=c_1(V_s+V_b),\qquad
c_1=c_0\frac{V_s}{V_s+V_b}.
$$

This denominator includes the sample itself. For the chosen $V_s=1\,\mathrm{mL}$ and $V_b=9\,\mathrm{mL}$, $c_1/c_0=1/10$, rather than $1/9$. Nine-tenths of the initial [solute](solute.md) is in the bath and one-tenth remains in the sample; nothing has vanished during equilibration.

Discarding the equilibrated bath removes its [solute](solute.md). A second fresh bath starts with only $c_1V_s$ of [solute](solute.md) in the entire system, so the same argument applies again. Induction gives the [geometric progression](geometric-progression.md)

$$
q=\frac{V_s}{V_s+V_b},\qquad
c_n=q c_{n-1}=c_0q^n,\qquad
\frac{c_n}{c_0}=10^{-n}\quad(V_s=1,\ V_b=9).
$$

Here $n$ counts completed equilibrations with fresh baths: $n=1$ is the first bath, $n=2$ follows one replacement, and $n=3$ follows two replacements. The normalized sample [concentrations](concentration.md) are respectively $0.1$, $0.01$ and $0.001$. Leaving the first bath in place for longer cannot lower the ideal equilibrium value below $0.1$.

<a id="image-repeated-fresh-baths-reduce-normalized-solute-concentration-geometrically"></a>
![](biochemical-dialysis-repeated-bath-model.png)

**[Figure 2](#image-repeated-fresh-baths-reduce-normalized-solute-concentration-geometrically). Repeated fresh baths reduce normalized solute concentration geometrically**. Original fixed-[volume](volume-thermodynamics.md) model, not experimental data. The left panel normalizes the first bath's conserved [amount of substance](amount-of-substance.md) by $c_0V_s$, distinguishing the sample's $0.1$ share from the bath's $0.9$ share. The right panel plots sample [solute](solute.md) [concentration](concentration.md) divided by $c_0$ after each completed fresh-bath equilibration on a logarithmic vertical axis. The [protein](protein-split.md) curve is normalized independently by its own initial [concentration](concentration.md). The perfectly retained [protein](protein-split.md) stays at normalized [concentration](concentration.md) one only because its [amount of substance](amount-of-substance.md) and the sample [volume](volume-thermodynamics.md) are fixed.

The same conservation argument handles a fresh bath already containing a permeant [solute](solute.md) at fixed [concentration](concentration.md) $b$:

$$
c_n=\frac{V_sc_{n-1}+V_bb}{V_s+V_b},\qquad
c_n-b=q(c_{n-1}-b),\qquad
c_n=b+(c_0-b)q^n.
$$

Thus the sample approaches $b$, not necessarily zero. For example, if a hypothetical new buffer component starts at zero in the sample and at $b$ in every bath, its sample [concentration](concentration.md) reaches $0.9b$, $0.99b$ and $0.999b$ in the three equilibrations. Outward removal and inward replacement follow the same mathematics.

Equilibrium fractions do not specify elapsed time. An illustrative well-mixed [linear ordinary differential equation](linear-ordinary-differential-equation-split.md) model within one bath is

$$
V_s\frac{dc_s}{dt}=-K(c_s-c_b),\qquad
V_b\frac{dc_b}{dt}=K(c_s-c_b),\qquad K>0.
$$

Here $K$ is an effective transfer coefficient with units of [volume](volume-thermodynamics.md) per time. Adding the two equations conserves $V_sc_s+V_bc_b$; subtracting their normalized forms gives

$$
\frac{d(c_s-c_b)}{dt}=-K\left(\frac1{V_s}+\frac1{V_b}\right)(c_s-c_b).
$$

The difference undergoes [exponential decay](exponential-decay.md). A bath replacement resets $c_b$, renewing the driving difference without making $c_s$ jump instantly. The plotted points are equilibrium endpoints, not a measured time course or a timetable for an arbitrary [protein](protein-split.md).

Real sample [volume](volume-thermodynamics.md) can change through [osmosis](osmosis.md); [proteins](protein-split.md) can be lost through leakage or [adsorption](adsorption.md) to the [semipermeable membrane](semipermeable-membrane.md). Consequently, a measured decrease in [protein](protein-split.md) [concentration](concentration.md) alone cannot distinguish dilution from loss of [protein](protein-split.md). Measuring recovered [volume](volume-thermodynamics.md) as well as [protein](protein-split.md) [concentration](concentration.md) permits an estimate of recovered [protein](protein-split.md) [mass](mass.md).[Tech Tip 20, p. 2, Other Factors in Dialysis: water transport, volume change and nonspecific membrane binding](dialysis-an-overview-pierce-biotechnology-technical-note.md)

## ↑ Ancestors (4)

1. [Dialysis (biochemistry)](dialysis-biochemistry.md)
2. [Biochemistry](biochemistry-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)
