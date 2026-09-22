# SEC molar mass calibration

↑ **Parent:** [Size-exclusion chromatography](size-exclusion-chromatography.md)

[SEC molar mass calibration](sec-molar-mass-calibration.md) measures standards under the same column, [solvent](solvent.md), and [temperature](temperature-split.md) conditions as the unknown. Over a suitable fractionation interval, a common empirical approximation is

$$
\log_{10}\!\left(\frac{M_{\rm app}}{M_{\rm ref}}\right)=a-bV_e,\qquad b>0,
$$

where $M_{\rm ref}$ specifies the [molar mass](molar-mass.md) unit and $b$ has inverse-[volume](volume-thermodynamics.md) units. Interpolation is conditional on the standards' size–[molar mass](molar-mass.md) relationship. [SEC](size-exclusion-chromatography.md) measures access associated with [hydrodynamic size](hydrodynamic-size.md), so a branched [polymer](polymer-split.md), an extended chain, and a compact [protein](protein-split.md) need not share that relationship.

<a id="image-size-exclusion-chromatography-theoretical-calibration"></a>
![](size-exclusion-chromatography-theoretical-calibration.png)

**[Figure 4](#image-size-exclusion-chromatography-theoretical-calibration). Theoretical SEC chromatogram peaks and a stipulated size-to-molar mass calibration**. Original model, not measured data: $V_0=5\,\mathrm{mL}$, $V_t=13\,\mathrm{mL}$, $K_d=\operatorname{clip}(1-\log_4(R_h/\mathrm{nm}),0,1)$, and standard-family $M=10^4(R_h/\mathrm{nm})^2\,\mathrm{g\,mol^{-1}}$. Equal-area [Gaussian distribution](normal-distribution.md) peaks have a chosen width $0.28\,\mathrm{mL}$ and equal detector response factors. The lower curve includes model exclusion and full-access plateaus; its secondary mass scale applies only to the stipulated standards.

In this model the $80{,}000$, $40{,}000$, and $20{,}000\,\mathrm{g\,mol^{-1}}$ standards have [hydrodynamic radii](hydrodynamic-radius.md) $2\sqrt2$, $2$, and $\sqrt2\,\mathrm{nm}$ and elute at $7$, $9$, and $11\,\mathrm{mL}$. An unknown at $8\,\mathrm{mL}$ would be assigned $M_{\rm app}=40{,}000\sqrt2\,\mathrm{g\,mol^{-1}}$ by this calibration. But a $40{,}000\,\mathrm{g\,mol^{-1}}$ species that expands from $2$ to $2\sqrt2\,\mathrm{nm}$ elutes at $7\,\mathrm{mL}$ and is assigned $80{,}000\,\mathrm{g\,mol^{-1}}$ without gaining any [mass](mass.md). The numbers demonstrate ambiguity, rather than predict a real unfolding transition.

Changes in [conformational isomerism](conformational-isomerism.md), [protein folding](protein-folding.md), [protein denaturation](denaturation-biochemistry.md), and [protein aggregation](protein-aggregation.md) can therefore shift peaks. Association usually increases size; compaction can reduce size at unchanged [molar mass](molar-mass.md). [Adsorption](adsorption.md) creates a different ambiguity: delayed elution need not indicate a smaller species. A different [solvent](solvent.md) can change both [polymer](polymer-split.md) coil dimensions and interactions with the packing. The [SEC protein conformation experiment](sec-protein-conformation-experiment.md) tests these alternatives with additional detectors.

## ↑ Ancestors (5)

1. [Size-exclusion chromatography](size-exclusion-chromatography.md)
2. [Liquid chromatography](liquid-chromatography.md)
3. [Chromatography](chromatography-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Hydrodynamic radius](hydrodynamic-radius.md)
- [Polystyrene](polystyrene.md)
- [SEC molar mass calibration](sec-molar-mass-calibration.md)
- [Size-exclusion chromatography](size-exclusion-chromatography.md)
- [Two-population molar mass example](two-population-molar-mass-example.md)
