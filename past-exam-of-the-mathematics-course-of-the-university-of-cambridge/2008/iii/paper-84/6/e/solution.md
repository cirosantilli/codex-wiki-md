<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume both openings have positive area, no imposed wind pressure, a light buoyant plume, and a [Boussinesq approximation](../../../../../../boussinesq-approximation.md). Write $S=\pi Q_s$ and $B_s=\pi F_s$ for physical source volume and buoyancy flux. Include [discharge coefficients](../../../../../../discharge-coefficient.md) $C_H,C_0$; if ideal openings are intended, set these to one. In a steady two-layer [displacement ventilation](../../../../../../displacement-ventilation.md) state with interface height $z_*$, let the floor inflow be $q_0$ and roof outflow $q_H$. Volume and buoyancy balances give

$$
q_H=q_0+S=\pi Q(z_*),
\qquad g'_u=\frac{B_s}{q_H}.
$$

The [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) head across the warm upper layer must equal the two opening losses:

$$
\frac{q_0^2}{2C_0^2A_0^2}
+\frac{q_H^2}{2C_H^2A_H^2}
=g'_u(H-z_*).
$$

A positive unprocessed lower layer needs $q_0>0$. At the boundary where this layer disappears, $z_*=0$, the plume can entrain no lower ambient fluid, so $q_0=0$, $q_H=S$ and $g'_u=B_s/S$. The critical condition is therefore $S^3=2C_H^2A_H^2B_sH$.

To determine the inequality, consider a fully processed room. Its steady [reduced gravity](../../../../../../reduced-gravity-split.md) is $g'=B_s/S$. If $p_0$ is the interior-to-exterior pressure difference at the floor, source-volume blocking of fresh floor inflow requires $p_0\ge0$. Both openings then exhaust, with

$$
S=C_0A_0\sqrt{2p_0/\rho_0}
+C_HA_H\sqrt{2(p_0/\rho_0+g'H)}.
$$

The right-hand side is increasing in $p_0$ and has its minimum at zero. Consequently a fully processed state exists exactly when

$$
\boxed{S^3\ge2C_H^2A_H^2B_sH,
\qquad Q_s^3\ge\frac{2C_H^2A_H^2F_sH}{\pi^2}.}
$$

This is [source-volume blocking of displacement ventilation](../../../../../../source-volume-blocking-of-displacement-ventilation.md). At equality floor inflow vanishes; above it the floor can also exhaust and no fresh lower-layer supply is needed. Below it, the floor pressure must be negative, admitting fresh fluid and supporting a positive lower layer. In fact the steady interface equation has a unique positive root: its loss side increases with $z_*$ because $Q(z_*)$ increases, while its buoyancy-head side decreases.

The floor-opening area affects the positive-interface state and its approach, but drops out of the blocking threshold because floor flux is zero at the threshold. Equal splitting of pressure head, or using a source-free effective opening area at this transition, would miss this distinction. If the floor opening is sealed, the fresh-inflow argument no longer applies: a finite source with only roof exhaust instead cycles the room asymptotically as in the ceiling-opening case of part (c).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
