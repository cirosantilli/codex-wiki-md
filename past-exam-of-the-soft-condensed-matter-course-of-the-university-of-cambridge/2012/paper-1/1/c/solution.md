<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For monovalent mobile ions, the linearized [Debye–Hückel screening length](../../../../../debye-huckel-screening-length.md) is

$$
\lambda^2=\frac{\epsilon_0\epsilon_r k_BT}{e^2\sum_i n_i z_i^2}.
$$

Here $n_i$ is a [number density](../../../../../number-density.md) in $\mathrm{m^{-3}}$, not a [molarity](../../../../../molar-concentration.md). Use the question's idealized neutral-water convention, $c_+=c_-=10^{-7}\,\mathrm{mol\,L^{-1}}$, and $T=293.15\,\mathrm K$. Both ion species contribute:

$$
\lambda=\sqrt{\frac{80\epsilon_0k_BT}{2e^2N_A\,10^3\times10^{-7}}},
\qquad \boxed{\lambda_{\rm water}\simeq9.63\times10^{-7}\,\mathrm m\simeq0.96\,\mu\mathrm m.}
$$

For added salt concentration $c_s$ in $\mathrm{mol\,L^{-1}}$, the [ionic strength](../../../../../ionic-strength.md) in this model is $I=c_s+10^{-7}\,\mathrm{mol\,L^{-1}}$. With the numerical [molarity](../../../../../molar-concentration.md) $I_M=I/(1\,\mathrm{mol\,L^{-1}})$,

$$
\lambda=\frac{0.3045\,\mathrm{nm}}{\sqrt{I_M}},\qquad
\boxed{c_s\simeq0.0927\,\mathrm{mol\,L^{-1}}\simeq0.093\,\mathrm M\quad(\lambda=1\,\mathrm{nm}).}
$$

The water contribution is negligible at that salt level. The factor $10^3$ converts molarity into $\mathrm{mol\,m^{-3}}$; omitting it or counting only one ion species gives a wrong screening [length](../../../../../length.md). Exact water autoionization and activities vary with [temperature](../../../../../temperature-split.md), so the first estimate uses the simplified neutral $10^{-7}\,\mathrm M$ concentrations implied by the question. At the higher salt level, ion-size effects, nonideal activities and changes in [permittivity](../../../../../permittivity-split.md) limit the numerical accuracy of this continuum estimate.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
