# Thermal transpiration experiment with a glass microtube

↑ **Parent:** [Thermal transpiration](thermal-transpiration.md)

Rojas Cardenas, Graur, Perrier and Méolans studied [thermal transpiration](thermal-transpiration.md) in [helium](helium.md) using a glass microtube of diameter $490\pm1\,\mathrm{\mu m}$ and length $3.05\pm0.01\,\mathrm{cm}$ in their 2012 experiment. They heated one reservoir, leaving the other near room [temperature](temperature-split.md), and measured tube-end [temperatures](temperature-split.md) of $300$ and $351\,\mathrm K$. Three contact [thermometers](thermometer.md) and an infrared camera checked the thermal conditions; the hot reservoir was warmer than the adjacent tube end, so heater [temperature](temperature-split.md) was not an adequate substitute for tube-end [temperature](temperature-split.md). Two [capacitance diaphragm gauges](capacitance-diaphragm-gauge.md) recorded the reservoir [pressures](pressure-split.md); a third gauge supported calibration. [Rojas Cardenas et al. (2012), An Experimental and Numerical Study of the Final Zero-Flow Thermal Transpiration Stage, §2.1](https://www.jstage.jst.go.jp/article/jtst/7/3/7_437/_pdf/-char/en#page=4)

<a id="image-thermal-transpiration-measurement-geometry-and-an-ideal-effusion-comparison"></a>
![](thermal-transpiration-bypass-and-flux.png)

**[Figure 2](#image-thermal-transpiration-measurement-geometry-and-an-ideal-effusion-comparison). Thermal-transpiration measurement geometry and an ideal effusion comparison**. The upper panel is a simplified apparatus schematic, not a reproduction of the experimental hardware. The lower panels compare one-way rates in a thin-hole toy model with $T_c=300\,\mathrm K$ and $T_h=351\,\mathrm K$; they are not measured capillary data.

Their earlier 2011 paper explains the measurement sequence. A wide bypass links the reservoirs in parallel with the microtube. After isolating the gas supply and pump, keep the bypass open to equalize [pressures](pressure-split.md) with the [temperature](temperature-split.md) difference already established. Closing the bypass defines $t=0$. The hot-side [pressure](pressure-split.md) rises and the cold-side [pressure](pressure-split.md) falls; ultimately their slopes approach zero at unequal [pressures](pressure-split.md). Repeating at different initial [pressures](pressure-split.md) changes the degree of rarefaction without changing the microtube. The 2011 study also compared [helium](helium.md) and [nitrogen](nitrogen.md) and imposed [temperature](temperature-split.md) differences of $50$, $60$ and $70\,\mathrm K$. [Rojas Cardenas et al. (2011), Thermal transpiration flow: A circular cross-section microtube submitted to a temperature gradient, measurement sequence](https://doi.org/10.1063/1.3561744)

The quantities to record are both $p_c(t)$ and $p_h(t)$, the reservoir volumes, and the [temperatures](temperature-split.md) relevant to their particle inventories. In an idealized reservoir of fixed volume $V_i$ and uniform fixed [temperature](temperature-split.md) $T_i$, the [ideal gas law](ideal-gas-law.md) gives $\dot N_i=[V_i/(k_BT_i)]\dot p_i$, so opposite inventory changes test particle conservation. If [temperature](temperature-split.md) changes, differentiation instead gives $\dot N_i=(V_i/k_B)[\dot p_i/T_i-p_i\dot T_i/T_i^2]$: a thermal drift can imitate particle transfer. The authors' 2011 presentation explicitly checks this thermal correction when extracting an initial [mass flow rate](mass-flow-rate.md) from the pressure slope. [Rojas et al., IUVSTA 2011 presentation, mass-flow extraction and thermal correction](https://www.itep.kit.edu/downloads/12_Rojas.pdf#page=25)

The 2012 paper compares the final [pressure](pressure-split.md) ratio across near-free-molecular through slip conditions with a kinetic model and empirical corrections. It does not establish the thin-hole square-root law at every measured [pressure](pressure-split.md). [Rojas Cardenas et al. (2012), abstract and comparison of final pressure ratios](https://www.jstage.jst.go.jp/article/jtst/7/3/7_437/_pdf/-char/en) For a replication, useful additional controls follow from the interpretation: remove the [temperature](temperature-split.md) difference to test the null signal; reverse it to test the direction; check gauge zero offsets and leaks; and wait for stable [temperatures](temperature-split.md) before closing the bypass. These are suggested controls, not claims that the cited paper performed each one. A reproducible pressure split at zero net transfer makes the failure of a single continuum wall model observable, while the [Knudsen number](knudsen-number.md) organizes which molecular and apparatus scales are competing.

**Table of contents**

- [Capacitance diaphragm gauge](capacitance-diaphragm-gauge.md)

## ↑ Ancestors (6)

1. [Thermal transpiration](thermal-transpiration.md)
2. [Kinetic theory](kinetic-theory-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
