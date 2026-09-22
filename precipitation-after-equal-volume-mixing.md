# Precipitation after equal-volume mixing

↑ **Parent:** [Solubility product](solubility-product.md)

Consider an original toy AB [salt](salt-chemistry.md) model with $K_{\mathrm{sp},c}=10^{-8}\,\mathrm M^2$ stipulated at fixed [temperature](temperature-split.md) and fixed [activity coefficient](activity-coefficient.md) product. This is a conditional concentration constant, not measured data for [calcium carbonate](calcium-carbonate.md) or any identified material. A stock contains A [cations](cation.md) and X [anions](anion.md); another contains Y [cations](cation.md) and B [anions](anion.md). All four [ions](ion.md) have unit [electric charge](electric-charge-split.md) magnitude. Only AB can form a [solid](solid.md); X and Y remain [spectator ions](spectator-ion.md). Assume full dissociation, no other [chemical reactions](chemical-reaction-split.md), and a mixed [volume](volume-thermodynamics.md) equal to the sum of the initial [volumes](volume.md).

Mix two stocks, each of [volume](volume-thermodynamics.md) $V$,, each at [molar concentration](molar-concentration.md) $C$ of its indicated [salt](salt-chemistry.md). Before any [precipitation](precipitation-chemistry.md), the mixed [volume](volume-thermodynamics.md) is $2V$, so

$$
c_{\mathrm A,0}=c_{\mathrm B,0}=\frac{CV}{2V}=\frac C2,\qquad Q_{c,0}=\frac{C^2}{4}.
$$

Multiplying the two stock [concentrations](concentration.md) would overestimate the mixed [ion product](ion-product.md) by a factor of four. The saturation threshold is $C=2\sqrt{K_{\mathrm{sp},c}}=2\times10^{-4}\,\mathrm M$.

If $C=10^{-4}\,\mathrm M$, mixing gives $Q_{c,0}=2.5\times10^{-9}\,\mathrm M^2<K_{\mathrm{sp},c}$: no AB [precipitate](precipitate.md) is favored. If $C=4\times10^{-4}\,\mathrm M$, mixing gives $Q_{c,0}=4\times10^{-8}\,\mathrm M^2>K_{\mathrm{sp},c}$. Suppose [nucleation](nucleation.md) occurs and bulk AB [solid](solid.md) remains at [chemical equilibrium](chemical-equilibrium.md). Equal starting inventories and one-to-one [stoichiometry](stoichiometry.md) require equal remaining [concentrations](concentration.md), hence

$$
c_{\mathrm A,eq}=c_{\mathrm B,eq}=\sqrt{K_{\mathrm{sp},c}}=10^{-4}\,\mathrm M,\qquad
\frac{n_{\mathrm{AB},s}}{2V}=\frac C2-10^{-4}\,\mathrm M=10^{-4}\,\mathrm M.
$$

For two $10\,\mathrm{mL}$ portions in the second case, each reacting [ion](ion.md) starts with $4\,\mathrm{\mu mol}$; the final $20\,\mathrm{mL}$ [chemical solution](solution-chemistry.md) retains $2\,\mathrm{\mu mol}$ of each, and $2\,\mathrm{\mu mol}$ of AB enters the [solid](solid.md). The respective X and Y inventories stay at $4\,\mathrm{\mu mol}$. Exactly half of each reacting inventory precipitates in this toy model.

<a id="image-precipitation-mixing-saturation-threshold"></a>
![](precipitation-mixing-saturation-threshold.png)

**[Figure 4](#image-precipitation-mixing-saturation-threshold). Equal-volume dilution changes the ion product before precipitation**. Original conditional AB model with $K_{\mathrm{sp},c}=10^{-8}\,\mathrm M^2$. Left: the two reacting-ion [concentrations](concentration.md) occupy different stocks and each halves on mixing. Right: the initial mixed [ion product](ion-product.md) relative to $K_{\mathrm{sp},c}$, with the two worked examples and saturation threshold. The curve is a model calculation, not measured cloudiness or a time trace.

The [chemical equilibrium](chemical-equilibrium.md) calculation adds a phase constraint to the inventory balance. Write $x=n_{\mathrm{AB},s}/(2V)$ and $c=C/2-x$. In the equilibrated bulk model,

$$
x\ge0,\qquad c\ge0,\qquad c^2\le K_{\mathrm{sp},c},\qquad x\bigl(K_{\mathrm{sp},c}-c^2\bigr)=0.
$$

When $x>0$, the last condition requires saturation; when $x=0$, the inventory can leave an undersaturated [chemical solution](solution-chemistry.md). Together these give $x=\max\{0,C/2-\sqrt{K_{\mathrm{sp},c}}\}$. This excludes a persistent [supersaturated solution](supersaturated-solution.md) by its explicit [chemical equilibrium](chemical-equilibrium.md) assumption; it does not model a [nucleation](nucleation.md) delay.

## ↑ Ancestors (5)

1. [Solubility product](solubility-product.md)
2. [Precipitation (chemistry)](precipitation-chemistry.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
