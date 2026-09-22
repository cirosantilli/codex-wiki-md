<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat the target as an absorbing sphere of effective capture radius $r_0$, surrounded by a uniform dilute reservoir of [RNA polymerase](../../../../rna-polymerase.md) with [number density](../../../../number-density.md) $C_\infty$. The steady [diffusion equation](../../../../diffusion-equation-split.md), [spherical symmetry](../../../../spherical-symmetry.md), and boundary conditions give

$$
\nabla^2 C=0,\qquad C(r_0)=0,\quad C(\infty)=C_\infty,
\qquad C(r)=C_\infty\left(1-\frac{r_0}{r}\right).
$$

By [Fick's laws](../../../../fick-s-laws.md), the inward capture rate per target is $4\pi r_0^2D_A C'(r_0)=4\pi D_A r_0C_\infty$. Multiplying by the target [number density](../../../../number-density.md) and comparing with the bimolecular [rate law](../../../../rate-law.md) therefore yields the [Smoluchowski association rate](../../../../smoluchowski-association-rate.md)

$$
\boxed{k_a=4\pi D_A r_0}.
$$

Its units here are $\mathrm{m^3\,s^{-1}}$, since the [concentrations](../../../../concentration.md) count particles rather than [moles](../../../../mole-unit.md). The absorbing boundary assumes every encounter is productive; orientation constraints would reduce the effective [association rate constant](../../../../association-rate-constant.md).

The [Stokes–Einstein relation](../../../../stokes-einstein-relation.md), for [RNA polymerase](../../../../rna-polymerase.md) radius $a=15\,\mathrm{nm}$ at an illustrative [temperature](../../../../temperature-split.md) $T=300\,\mathrm K$, gives

$$
D_A=\frac{k_BT}{6\pi\eta a}=1.46\times10^{-12}\,\mathrm{m^2\,s^{-1}}.
$$

Neither cell volume nor the effective $r_0$ is specified, so a unique numerical time is unavailable. A representative [Escherichia coli](../../../../escherichia-coli.md) volume is $V=1\,\mathrm{\mu m^3}=10^{-18}\,\mathrm{m^3}$. The $40$-[base pair](../../../../base-pair.md) target has a [DNA](../../../../deoxyribonucleic-acid.md) contour extent of about $40(0.34)=13.6\,\mathrm{nm}$; using this as an order-of-magnitude capture radius gives $k_a\simeq2.50\times10^{-19}\,\mathrm{m^3\,s^{-1}}$. For $M=3000$ independent searchers, the target's approximately constant encounter hazard is $Mk_a/V$, hence

$$
\boxed{\tau_3\simeq\frac{V}{Mk_a}=1.33\,\mathrm{ms}
\left(\frac{V}{1\,\mathrm{\mu m^3}}\right)
\left(\frac{13.6\,\mathrm{nm}}{r_0}\right)
\left(\frac{300\,\mathrm K}{T}\right)}.
$$

Using half the target's contour extent for $r_0$ instead gives about $2.7\,\mathrm{ms}$; the spherical capture model is not exact target geometry. One searcher's mean would be about $4\,\mathrm s$ under the first convention, whereas the first arrival among $3000$ is much faster.

If only a fraction $f_3=0.1$ of each searcher's time is available for three-dimensional [diffusion](../../../../diffusion.md), and nonspecific [DNA](../../../../deoxyribonucleic-acid.md) binding neither scans nor delivers the target, the effective searching population is $f_3M$. Thus $\boxed{\tau\simeq\tau_3/f_3=10\tau_3}$, about $13\,\mathrm{ms}$ under the stated estimate. This assumes stationarity, well-mixed searchers and no additional target-access route; nonspecific binding alone is sequestration, not [facilitated diffusion](../../../../facilitated-diffusion.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
