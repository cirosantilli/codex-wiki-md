<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The viscosity converts to $\eta=0.01\,\mathrm{Pa\,s}$, and the translation speed is $U=10^{-8}\,\mathrm{m\,s^{-1}}$. Mechanical power is $P_{\rm motor}=\zeta_{\rm chain}U^2$. The [hydrodynamic drag models for a polymer](../../../../../../hydrodynamic-drag-models-for-a-polymer.md) show why a conformation assumption is necessary.

For a largely aligned slender filament translating along its axis in unbounded fluid, use

$$
\zeta_\parallel\simeq\frac{2\pi\eta L}{\log(2L/a)-1/2},\qquad a=d/2=5\times10^{-10}\,\mathrm m.
$$

With $L=100\,\mathrm m$, $\log(2L/a)=\log(4\times10^{11})=26.715$, so $\zeta_\parallel\simeq0.240\,\mathrm{kg\,s^{-1}}$. The required [force](../../../../../../force.md) is about $2.4\times10^{-9}\,\mathrm N$, and

$$
\boxed{P_{\rm motor}\simeq2.4\times10^{-17}\,\mathrm W\quad\text{for aligned axial translation}.}
$$

Transverse translation has roughly twice the leading logarithmic drag. This estimate treats the entire contour as an aligned slender body, assumes creeping flow, and omits bead drag, wall corrections, and additional motor losses. It is not a drag formula for an unstretched coil.

For an alternative nondraining coil, approximate the hydrodynamic radius by its [radius of gyration](../../../../../../radius-of-gyration.md), $R_h\sim R_g\simeq\sqrt{Ll_p/3}=8.16\times10^{-4}\,\mathrm m$. The [Stokes drag law](../../../../../../stokes-s-law.md) gives $\zeta\sim6\pi\eta R_h=1.54\times10^{-4}\,\mathrm{kg\,s^{-1}}$ and $P\sim1.54\times10^{-20}\,\mathrm W$. A freely draining toy model that sums $N$ spherical-monomer drags of radius $a$ instead gives $P=N6\pi\eta aU^2\simeq9.42\times10^{-17}\,\mathrm W$. Hydrodynamic interactions are suppressed in this last model. These distinct answers explain the need to specify conformation and hydrodynamic coupling; the stated data do not select a unique one.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
