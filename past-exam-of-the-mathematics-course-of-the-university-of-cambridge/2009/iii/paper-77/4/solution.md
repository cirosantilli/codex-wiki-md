<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\mathbf v$ be horizontal iceberg velocity, $\mathbf u_a$ the wind and $\mathbf u_w$ the current. Air and water [drag forces](../../../../../drag-physics.md) act on the relative velocities, typically with magnitudes proportional to their squares. Their exposed and immersed areas and drag coefficients differ. For iceberg mass $m$, the horizontal balance can be written schematically as

$$
m\left(\dot{\mathbf v}+f\hat{\mathbf z}\times\mathbf v\right)=\mathbf F_a(\mathbf u_a-\mathbf v)+\mathbf F_w(\mathbf u_w-\mathbf v)-mg\nabla\zeta,
$$

where $f$ is the [Coriolis parameter](../../../../../coriolis-parameter.md) and $\zeta$ the sea-surface elevation. The last term represents the large-scale [pressure gradient](../../../../../pressure-gradient.md); contact with pack ice and grounding require additional forces. [Iceberg free drift](../../../../../iceberg-free-drift.md) neglects such contact constraints, not the water drag or [Coriolis force](../../../../../coriolis-force.md).

In still water with a fixed wind force $\mathbf F$, a transparent transient model linearizes water drag as $-m\gamma\mathbf v$. Put $J\mathbf v=\hat{\mathbf z}\times\mathbf v$. Then

$$
\dot{\mathbf v}+(\gamma I+fJ)\mathbf v=\frac{\mathbf F}{m},\qquad\mathbf v_\infty=\frac{\gamma\mathbf F-fJ\mathbf F}{m(\gamma^2+f^2)}.
$$

The [damped free drift of an iceberg](../../../../../damped-free-drift-of-an-iceberg.md) is

$$
\boxed{\mathbf v(t)=\mathbf v_\infty+e^{-\gamma t}R(-ft)\bigl[\mathbf v(0)-\mathbf v_\infty\bigr].}
$$

Thus an initially resting berg accelerates under the wind, turns under the [Coriolis force](../../../../../coriolis-force.md), and approaches a balance of wind, water drag and rotation through damped [inertial oscillations](../../../../../inertial-oscillation.md). Its equilibrium drift is to the right of the wind in the Northern Hemisphere and to the left in the Southern Hemisphere. With quadratic drag, the drag coefficient in the equilibrium balance depends on speed; the linear formula illustrates the turning and relaxation rather than prescribing an exact percentage of wind speed.

For a moving ocean, the background [pressure gradient](../../../../../pressure-gradient.md) associated with [geostrophic balance](../../../../../geostrophic-balance.md) must also be included. Large tabular [icebergs](../../../../../iceberg.md) have substantial submerged area and respond strongly to currents; smaller bergs can have a larger wind-driven velocity relative to the water. Near Antarctica, the mainly westward [Antarctic Coastal Current](../../../../../antarctic-coastal-current.md) can carry bergs along the continental margin. Export into offshore gyres and then the eastward [Antarctic Circumpolar Current](../../../../../antarctic-circumpolar-current.md) changes their trajectories; bathymetry, winds, fronts and evolving size all matter. [Gladstone and Bigg's Weddell Sea tracking](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/D358D428FAADC2EE6FBAEFE94BA1B83A/S0954102002000032a.pdf/satellite_tracking_of_icebergs_in_the_weddell_sea.pdf) illustrates the contrast between coastal and offshore drift. The [Antarctic Convergence](../../../../../antarctic-convergence.md) separates colder Antarctic surface water from warmer water farther north, where an exported iceberg can encounter enhanced melting. No single wind direction determines the complete route.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
