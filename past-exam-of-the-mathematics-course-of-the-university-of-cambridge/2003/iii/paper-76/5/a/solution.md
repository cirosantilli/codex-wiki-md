<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the flux normalization of the supplied equations, with the common factor $\pi$ suppressed. Put $q=wb^2$, $m=w^2b^2$ and $B_0=g'q$. The [top-hat plume model](../../../../../../top-hat-plume-model.md) reduces to

$$
q'=2\alpha\sqrt m,\qquad m'=B_0q/m,\qquad B_0'=0.
$$

Eliminate height to obtain $dm/dq=B_0q/(2\alpha m^{3/2})$. Integrating with zero source volume and momentum flux gives the [pure plume balance](../../../../../../pure-plume-balance.md)

$$
m^{5/2}=\frac{5B_0}{8\alpha}q^2.
$$

Equivalently, seek $b=dz$ and $w=sz^{-1/3}$. The volume balance gives $d=6\alpha/5$, and the momentum and buoyancy balances give $g'=(4s^2/3)z^{-5/3}$ and $B_0=4d^2s^3/3$. Thus

$$
\boxed{b=\frac{6\alpha}{5}z,\qquad
w=\left(\frac{25B_0}{48\alpha^2}\right)^{1/3}z^{-1/3},\qquad
g'=\frac43\left(\frac{25B_0}{48\alpha^2}\right)^{2/3}z^{-5/3}.}
$$

A finite source replaces the singular point origin by a [plume virtual origin](../../../../../../plume-virtual-origin.md) and source conditions. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) requires the fractional density difference to be small, so density can be replaced by ambient density in inertia and entrainment while retaining the small difference in buoyancy. In this solution it requires $g'/g\ll1$. The approximation necessarily fails sufficiently near the ideal point source, where $g'$ diverges, and can also fail for strongly heated or otherwise large-density-contrast sources. The similarity solution is appropriate farther away once entrainment has diluted the anomaly, assuming a uniform ambient, constant entrainment coefficient and negligible confinement, heat loss and stratification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
