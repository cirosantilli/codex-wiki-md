<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $r=a_{\rm ADP}/a_{\rm ATP}$ and use a one-molar [standard state](../../../../standard-state.md), so the [inorganic phosphate](../../../../inorganic-phosphate.md) activity is approximately $a_P=0.006$. With the source's stated standard [hydrolysis](../../../../hydrolysis.md) value,

$$
\Delta G_{\rm hyd}=-50{,}000+RT\ln(0.006r)\quad\mathrm{J\,mol^{-1}}.
$$

The downhill proton-transfer [Gibbs free energy](../../../../gibbs-free-energy.md) is $F\Delta p$ for the signed driving [force](../../../../force-split.md) $\Delta p=-0.150$ V. Ideal reversible balance of one complete turn requires

$$
-3\Delta G_{\rm hyd}+10F\Delta p=0,
\qquad \Delta G_{\rm hyd}=\frac{10}{3}F\Delta p=-48.243\ \mathrm{kJ\,mol^{-1}}.
$$

Solving yields

$$
\boxed{r=\frac1{0.006}\exp\!\left[\frac{50{,}000+(10/3)F\Delta p}{RT}\right]
\simeq3.29\times10^2\quad(T=310.15\ \mathrm K).}
$$

At 298.15 K the estimate is $3.39\times10^2$. [Temperature](../../../../temperature-split.md) is not specified in this paragraph; the first value explicitly adopts physiological [temperature](../../../../temperature-split.md) rather than pretending it is supplied. The unexpectedly large [ADP](../../../../adenosine-diphosphate.md)/[ATP](../../../../adenosine-triphosphate.md) ratio follows from using the **printed standard** value $-50$ kJ/mol with the stated dilute [inorganic phosphate](../../../../inorganic-phosphate.md). One must not silently replace that value by another convention or treat it as the already concentration-corrected cellular [hydrolysis](../../../../hydrolysis.md) [Gibbs free energy](../../../../gibbs-free-energy.md).

This estimate assumes ideal [thermodynamic activities](../../../../thermodynamic-activity.md), consistent [pH](../../../../ph.md) and [magnesium](../../../../magnesium.md) conventions, tight coupling of ten [protons](../../../../proton.md) to three [ATP](../../../../adenosine-triphosphate.md), no leak or transport overhead, and operation close to reversible balance. A working cell is not in global equilibrium. Net synthesis at this fixed driving [force](../../../../force-split.md) requires $\Delta G_{\rm turn}<0$, hence $r$ **above** this reversible-balance threshold; finite [chemical kinetics](../../../../chemical-kinetics-split.md) and dissipation prevent the [stoichiometry](../../../../stoichiometry.md) alone from determining an exact physiological ratio.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
