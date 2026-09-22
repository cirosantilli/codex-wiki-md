# Chemostat

↑ **Parent:** [Mathematical biology](mathematical-biology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemostat)

A [chemostat](chemostat.md) maintains a well-mixed culture at constant volume $V$ by feeding fresh nutrient solution and removing culture at the same volumetric flow $Q$. Its [dilution rate](dilution-rate.md) is $D=Q/V$. Mixing makes the outflow's nutrient [concentration](concentration.md) and [biomass concentration](biomass-concentration.md) equal to those inside the vessel; continuous replacement supplies nutrient and also removes growing cells.

The simplest one-nutrient [chemostat](chemostat.md) uses nutrient [concentration](concentration.md) $s(t)$, [biomass concentration](biomass-concentration.md) $x(t)$, constant feed nutrient [concentration](concentration.md) $s_{\mathrm{in}}>0$, and constant [biomass yield](biomass-yield.md) $Y>0$. Assume a cell-free feed, one growth-limiting nutrient, constant volume, and no cell retention, death or additional nutrient consumption for maintenance. With [specific growth rate](specific-growth-rate.md) $\mu(s)$, its [ordinary differential equations](ordinary-differential-equation.md) are

$$
\frac{\mathrm{d}s}{\mathrm{d}t}=D(s_{\mathrm{in}}-s)-\frac{\mu(s)x}{Y},\qquad
\frac{\mathrm{d}x}{\mathrm{d}t}=(\mu(s)-D)x.
$$

The nutrient balance contains inflow $Ds_{\mathrm{in}}$, outflow $Ds$, and consumption $\mu(s)x/Y$; the biomass balance contains production $\mu(s)x$ and removal $Dx$. If $s$ is in grams of nutrient per litre and $x$ in grams of dry biomass per litre, $Y$ is grams of dry biomass produced per gram of nutrient consumed. Thus both balances have units of their respective [concentration](concentration.md) per time. The [Monod equation](monod-equation.md) supplies an empirical choice of $\mu(s)$; the balances themselves express the stated production, consumption and transport assumptions.

The appeal of a [chemostat](chemostat.md) is that, at a positive [chemostat steady state](chemostat-steady-state.md), adjusting the pump sets the [specific growth rate](specific-growth-rate.md) to $D$. The residual nutrient [concentration](concentration.md) then adjusts to that rate, and the available nutrient together with [biomass yield](biomass-yield.md) sets the [biomass concentration](biomass-concentration.md). This gives a controlled way to compare cultures at selected growth rates and a simple quantitative warning of [chemostat washout](chemostat-washout.md).

Two 1950 publications on continuous culture are Novick and Szilard's Description of the Chemostat, Science 112(2920), 715-716, dated 15 December, and Monod's La technique de culture continue. Théorie et applications, Annales de l'Institut Pasteur 79, 390-410. The latter's original bibliographic details are reproduced in the contents of Monod's collected papers. These references identify contemporary publications without establishing priority between them. [Aaron Novick and Leo Szilard, Description of the Chemostat (1950)](https://doi.org/10.1126/science.112.2920.715). [Monod's 1950 original, listed in Selected Papers in Molecular Biology by Jacques Monod, contents p. vi](https://api.pageplace.de/preview/DT0400.9780323142632_A23647608/preview-9780323142632_A23647608.pdf).

**Table of contents**

- [Biomass concentration](biomass-concentration.md)
- [Biomass yield](biomass-yield.md)
- [Chemostat steady state](chemostat-steady-state.md)
- [Chemostat washout](chemostat-washout.md)
- [Monod chemostat equilibrium and relaxation](monod-chemostat-equilibrium-and-relaxation.md)
- [Dilution rate](dilution-rate.md)

## ↑ Ancestors (4)

1. [Mathematical biology](mathematical-biology-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Biomass concentration](biomass-concentration.md)
- [Biomass yield](biomass-yield.md)
- [Chemostat](chemostat.md)
- [Chemostat steady state](chemostat-steady-state.md)
- [Chemostat washout](chemostat-washout.md)
- [Dilution rate](dilution-rate.md)
- [Mathematical biology](mathematical-biology-split.md)
- [Monod chemostat equilibrium and relaxation](monod-chemostat-equilibrium-and-relaxation.md)
- [Monod equation](monod-equation.md)
- [Specific growth rate](specific-growth-rate.md)
