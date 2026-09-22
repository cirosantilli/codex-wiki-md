<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Illustration TODO.** The source's two-volume circulation sketch on page 4 is unavailable. Its exact arrows and layout cannot be recovered. The surviving flow law, [salinity](../../../../salinity.md)/[temperature](../../../../temperature-split.md) definitions and printed steady polynomial allow the calculation below under an explicit freshwater sign convention; no unavailable diagram values are invented.

Use $\Delta T=T_2-T_1>0$, $\Delta S=S_2-S_1$, and let positive $q$ be the thermally driven state with cold box 1 denser than warm box 2. Take positive $F$ to freshen box 1, represented in a fixed-volume [salt budget](../../../../salt-budget.md) by an equivalent salt removal $FS_1$ from that box and addition to the other reservoir. This is the freshwater convention compatible with the printed $+BF$ and positive $B$. It can represent a compensating saline [volume](../../../../volume.md) transfer or the usual virtual-salt-flux approximation. The exact pipe assignment is not claimed to have been read from the missing illustration.

Exchange in either circulation direction reduces a [salinity](../../../../salinity.md) difference at rate proportional to $|q|\Delta S$. Steady salt balance therefore gives

$$
\boxed{|q|\Delta S=FS_1,\qquad \Delta S=\frac{FS_1}{|q|}}\qquad(q\ne0).
$$

The supplied linear [equation of state](../../../../equation-of-state.md) gives

$$
\frac{\rho_1-\rho_2}{\rho_0}=\alpha\Delta T-\beta\Delta S,
\qquad q=k(\alpha\Delta T-\beta\Delta S).
$$

Eliminating $\Delta S$ yields the [two-box overturning model](../../../../two-box-overturning-model.md) equation

$$
\boxed{q|q|-A|q|+BF=0,\qquad A=k\alpha\Delta T,\qquad B=k\beta S_1}.
$$

Here $A$ and $B$ both have transport units when $q,F,k$ do, while $\alpha\Delta T$ and $\beta S_1$ are dimensionless. Although the source calls $q$ a mass flow, its stated Sverdrup units are [volume](../../../../volume.md) per time; the common reference [density](../../../../density.md) cancels in the Boussinesq salt/[volume](../../../../volume.md) approximation. At $F>0$, $q=0$ cannot be a finite-salinity steady state in this model. At $F=0$, zero flow needs separate treatment instead of division by $|q|$.

The circulation weakens when freshwater freshens the cold reservoir, and the weaker circulation removes the resulting [salinity](../../../../salinity.md) contrast less effectively. This [salt-advection feedback](../../../../salt-advection-feedback.md) is the mechanism behind multiple steady states, not an additional externally imposed switch.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
