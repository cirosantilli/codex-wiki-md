<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $h(t)$ for the height of the [filling-box first front](../../../../../filling-box-first-front.md) above the floor and $P(h)$ for the upward plume [volume flux](../../../../../volumetric-flow-rate.md) crossing it. Neglect the plume's horizontal area compared with $A$, use the [Boussinesq approximation](../../../../../boussinesq-approximation.md), and measure [buoyancy](../../../../../buoyancy.md) relative to the initially unmodified ambient. The first front separates fluid already modified by plume discharge from the unmodified fluid below; the entire upper region need not be uniformly mixed during an unventilated [filling box model](../../../../../filling-box-model.md) transient.

A finite injected [volume flux](../../../../../volumetric-flow-rate.md) $Q$ cannot enter a hermetically sealed, fixed-volume room under the [incompressible flow](../../../../../incompressible-flow.md) assumption. If $Q>0$, an equal overflow or exhaust is needed. Taking that exhaust at the ceiling, [volume conservation](../../../../../volume-conservation.md) of the region above the front gives

$$
-A\dot h=P(h)-Q,\qquad \boxed{\text{downward front speed}=\frac{P(h)-Q}{A}.}
$$

The source [volume flux](../../../../../volumetric-flow-rate.md) is subtracted because only entrained room fluid is removed from the initially unmodified region. The printed [pure plume](../../../../../pure-plume.md) law has $P(0)=0$, so it cannot be an exact finite-$Q$ source law down to the physical floor. In the far field where $Q\ll P(h)$, or for a heat source whose injected [volume flux](../../../../../volumetric-flow-rate.md) is negligible, it gives

$$
\boxed{-\dot h\simeq\frac{\lambda B^{1/3}}A h^{5/3}},\qquad h(t)=\left[H^{-2/3}+\frac{2\lambda B^{1/3}}{3A}t\right]^{-3/2}.
$$

Here $t=0$ is when the plume discharge first reaches the ceiling. Retaining $Q$ while using the far-field law gives $-\dot h=[\lambda B^{1/3}h^{5/3}-Q]/A$ only while that law remains a valid approximation; it must not be extrapolated to predict negative plume entrainment. A [plume virtual origin](../../../../../plume-virtual-origin.md) below the floor is one way to match a nonzero source [volume flux](../../../../../volumetric-flow-rate.md).

For [displacement ventilation](../../../../../displacement-ventilation.md), let $F$ be the total ceiling exhaust, $S$ the total buoyant-source [volume flux](../../../../../volumetric-flow-rate.md), and $L=F-S$ the separate ambient inflow into the lower layer. [Volume conservation](../../../../../volume-conservation.md) and the upper-layer [buoyancy flux](../../../../../buoyancy-flux.md) balance give

$$
A\dot h=F-P(h),\qquad \frac{d}{dt}\bigl[A(H-h)b\bigr]=B-Fb.
$$

The ambient inflow has zero reference [buoyancy](../../../../../buoyancy.md). In the ideal two-layer closure the upper layer is uniformly mixed with [reduced gravity](../../../../../reduced-gravity-split.md) $b>0$, and the lower layer has zero reference [buoyancy](../../../../../buoyancy.md). The plume supplies the upper layer while lighter upper-layer air is removed at the ceiling. An interface is driven downward when $P(h)>F$ and upward when $P(h)<F$; since $P'(h)>0$, its equilibrium is stable.

In the negligible-source-volume [pure plume](../../../../../pure-plume.md) limit, identifying $F=Q_v$ gives the intended one-source answer

$$
\boxed{h_1=\left(\frac{Q_v}{\lambda B^{1/3}}\right)^{3/5},\qquad b_1=\frac B{Q_v}.}
$$

The prescribed inequality makes $h_1/H\ll1$, so both layers fit in the room. It does not, by itself, justify neglecting a finite source $Q$: the [pure plume](../../../../../pure-plume.md) source region must also be small compared with $h_1$, normally requiring $Q\ll Q_v$. If $Q_v$ denotes additional background ventilation rather than total exhaust, replace $Q_v$ in both formulas by $Q+Q_v$. If it is total exhaust, the separate ambient inlet carries $Q_v-Q$. These conventions must not be mixed.

For $n$ independent equal [axisymmetric pure plumes](../../../../../axisymmetric-pure-plume.md), adding their [volume fluxes](../../../../../volumetric-flow-rate.md) gives

$$
P_n(h)=n\lambda(B/n)^{1/3}h^{5/3}=\lambda n^{2/3}B^{1/3}h^{5/3}.
$$

Thus the conventional [multiple-plume displacement ventilation](../../../../../multiple-plume-displacement-ventilation.md) calculation with negligible source [volume flux](../../../../../volumetric-flow-rate.md) and separate ambient ventilation gives

$$
\boxed{h_n=n^{-2/5}h_1,\qquad b_n=\frac B{Q_v}.}
$$

Splitting the [buoyancy flux](../../../../../buoyancy-flux.md) increases total [fluid entrainment](../../../../../fluid-entrainment.md), so the same ventilation balances the plumes at a lower interface. The global [buoyancy flux](../../../../../buoyancy-flux.md) is unchanged, which leaves the upper-layer [reduced gravity](../../../../../reduced-gravity-split.md) unchanged. Independence requires sufficiently separated sources and plumes that do not merge below the interface.

There is, however, a substantive problem with the literal source-volume specification in this paragraph of the PDF. It puts all $Q_v$ through the buoyant sources, so $S=F=Q_v$ and $L=0$. For every positive interface height, entraining plumes have

$$
P_n(h)=Q_v+E(h),\qquad E(h)>0,\qquad A\dot h=-E(h)<0.
$$

There is no fresh ambient inflow to replace the lower-layer fluid being entrained. Consequently **the stated positive steady two-layer configuration does not follow from those literal hypotheses**. This is [no steady displacement layer without ambient supply](../../../../../no-steady-displacement-layer-without-ambient-supply.md), not a small correction to the $n^{-2/5}$ scaling. For example, a matched [plume virtual origin](../../../../../plume-virtual-origin.md) gives

$$
P_n(h)=C_n(h+z_0)^{5/3},\quad C_n=\lambda n^{2/3}B^{1/3},\quad z_0=(S/C_n)^{3/5},\quad h_*=(F/C_n)^{3/5}-z_0.
$$

When $S=F$, this yields $h_*=0$. The unshifted answer $h_n$ equals the omitted $z_0$ in this case, so neglecting the source region cannot be justified. Also each source has reference [buoyancy](../../../../../buoyancy.md) $(B/n)/(Q_v/n)=B/Q_v$, already equal to the proposed upper-layer value; a steady positive plume cannot entrain zero-buoyancy lower fluid and still deliver that same value. The conventional answer is valid for a corrected arrangement with negligible-volume buoyancy sources and a separate ambient inlet, or with source flux $S<Q_v$ and the remaining $Q_v-S$ supplied directly to the lower layer. A real room may have other circulation or continuous stratification, but that requires a different model.

For the intended [displacement ventilation](../../../../../displacement-ventilation.md) model, reducing the exhaust to $F=Q_v/2$ makes the new equilibrium

$$
h_*=2^{-3/5}h_n,\qquad b_* =\frac{2B}{Q_v}.
$$

The interface initially descends since its old plume [volume flux](../../../../../volumetric-flow-rate.md) exceeds the new exhaust. In [ventilated filling-box relaxation](../../../../../ventilated-filling-box-relaxation.md), writing $V_*=A(H-h_*)$ and taking the [linearization](../../../../../linearization.md) of the two balances above gives

$$
\delta\dot h=-\frac{P_n'(h_*)}{A}\delta h,\qquad \delta\dot b=-\frac F{V_*}\delta b-\frac{b_*P_n'(h_*)}{V_*}\delta h.
$$

As $P_n'(h_*)=5F/(3h_*)$, the two decay times are

$$
\tau_h=\frac{3Ah_*}{5F}=\frac{6Ah_*}{5Q_v},\qquad \tau_b=\frac{A(H-h_*)}{F}=\frac{2A(H-h_*)}{Q_v}.
$$

A [dimensional analysis](../../../../../dimensional-analysis.md) estimate of the full adjustment time is therefore

$$
\boxed{t_{\mathrm{adjust}}\sim\max(\tau_h,\tau_b)\sim\frac{2AH}{Q_v}\quad(h_*\ll H).}
$$

The interface adjusts on the shorter lower-layer scale; replacing the [buoyancy](../../../../../buoyancy.md) stored throughout the upper layer is slower. Exact equilibrium is approached asymptotically, and a specified small relative tolerance adds a logarithmic factor. For the literal all-inflow-through-sources arrangement there is no positive two-layer equilibrium to return to; $2AH/Q_v$ is only a flushing-scale estimate for a different, whole-room adjustment.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 345](../../paper-345-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
