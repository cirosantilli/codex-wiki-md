<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use high-resolution [quasar](../../../../../../quasar.md) spectra to fit [Voigt profiles](../../../../../../voigt-profile.md) to [Lyman-alpha forest](../../../../../../lyman-alpha-forest.md) lines near $z=3$, where the transition appears near $121.6(1+3)\simeq486.4\,\mathrm{nm}$. Each fit estimates the neutral-hydrogen [column density](../../../../../../column-density.md) and the velocity-width parameter $b$. The one-dimensional [Maxwell-Boltzmann velocity distribution](../../../../../../maxwell-boltzmann-velocity-distribution.md) has variance $k_BT/m_{\rm H}$; consequently the thermal optical-depth profile is proportional to $\exp[-(v-v_0)^2/b^2]$, with the [thermal cutoff of Lyman-alpha line widths](../../../../../../thermal-cutoff-of-lyman-alpha-line-widths.md)

$$
\boxed{b_{\rm th}^2=\frac{2k_BT}{m_{\rm H}},
\qquad T=\frac{m_{\rm H}b_{\rm th}^2}{2k_B}.}
$$

For example, a purely thermal $b=20\,\mathrm{km\,s^{-1}}$ corresponds to $T\simeq2.4\times10^4\,\mathrm K$.

An observed broad line is not by itself a thermometer: [peculiar velocities](../../../../../../peculiar-velocity.md), bulk gradients, blending and instrumental resolution also broaden it. For independent Gaussian contributions, $b^2=b_{\rm th}^2+b_{\rm nonthermal}^2+b_{\rm inst}^2$. After modeling the instrumental response, an uncorrected total width gives an upper bound on the thermal [temperature](../../../../../../temperature.md), not a lower bound. The narrowest lines at each [column density](../../../../../../column-density.md) are least affected by additional broadening. Their lower envelope in the $b$–$N_{\rm HI}$ plane constrains the [temperature-density relation of photoionized intergalactic gas](../../../../../../temperature-density-relation-of-photoionized-intergalactic-gas.md), often written $T=T_0(1+\delta)^{\gamma-1}$.

Calibrate the conversion between [column density](../../../../../../column-density.md), density and width with hydrodynamic models incorporating the [cosmic ionizing background](../../../../../../cosmic-ionizing-background.md), pressure smoothing, resolution and selection. It estimates $T_0$ and the slope rather than assigning one [temperature](../../../../../../temperature.md) to every absorber. Where aligned metal lines trace the same gas, comparing species of different atomic mass can separately estimate a common nonthermal contribution because thermal $b^2$ scales as $m^{-1}$. The forest lower-envelope method and its numerical calibration are developed in [Schaye and collaborators' temperature analysis](https://arxiv.org/abs/astro-ph/9906271).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
