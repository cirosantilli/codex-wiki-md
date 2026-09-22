<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $q_b$ be floor inflow and $q_t$ roof outflow. Use effective-area discharge $A\sqrt{\delta p/\rho}$, matching the factors in the supplied relations. With negligible source volume, both equal $q$. The lower region has exterior [mass density](../../../../../density.md) while the warm upper layer has [reduced gravity](../../../../../reduced-gravity-split.md) $g'$ and depth $H-h$. [hydrostatic pressure](../../../../../hydrostatic-pressure.md) therefore supplies a total opening [pressure](../../../../../pressure.md) head $g'(H-h)$. Equal openings sharing equal discharge take half each, giving

$$
q=A\sqrt{\frac{g'(H-h)}2}.
$$

Steady lower-layer volume conservation sets this ventilation rate equal to the entrained [turbulent plume](../../../../../turbulent-plume-split.md) flux at the interface, $q=\lambda B^{1/3}h^{5/3}$. Upper-layer buoyancy conservation gives $B=qg'$. These are the required balances for [displacement ventilation](../../../../../displacement-ventilation.md):

$$
\boxed{A\sqrt{\frac{g'(H-h)}2}=\lambda B^{1/3}h^{5/3},\qquad
B=Ag'\sqrt{\frac{g'(H-h)}2}}.
$$

Eliminating $g'$ and $q$ gives the [displacement-ventilation interface height](../../../../../displacement-ventilation-interface-height.md) equation

$$
\boxed{2\lambda^3h^5=A^2(H-h)},\qquad
\boxed{\frac{\zeta^5}{1-\zeta}=\frac{A^2}{2\lambda^3H^4},\quad\zeta=\frac hH\in(0,1)}.
$$

The left side is strictly increasing from zero to infinity, so there is one interface height. It depends on opening geometry and plume entrainment, not on $B$; the resulting $g'=B^{2/3}/(\lambda h^{5/3})$ and throughflow do depend on $B$.

For finite source volume $Q$, conservation instead gives $q_t=q_b+Q$. The two [pressure](../../../../../pressure.md) drops are no longer equal:

$$
\frac{q_b^2+q_t^2}{A^2}=g'(H-h),\qquad B=q_tg'.
$$

Let $q_p(h;Q)$ be a physically entraining source plume: $q_p(0;Q)=Q$ and $q_p(h;Q)>Q$ for $h>0$. Its interface balance is $q_p=q_t=Q+q_b$. Therefore, as $q_b$ reaches zero, a positive-depth lower layer has no replenishment and cannot remain steady: this is [no steady displacement layer without ambient supply](../../../../../no-steady-displacement-layer-without-ambient-supply.md). The limiting interface is $h=0$. At the threshold $q_t=Q$ and $g'=B/Q$, and the entire hydrostatic head drives the roof discharge. Hence

$$
\boxed{Q_c=A\sqrt{\frac{BH}{Q_c}},\qquad Q_c=(A^2BH)^{1/3}}.
$$

This is [source-volume blocking of displacement ventilation](../../../../../source-volume-blocking-of-displacement-ventilation.md). The half-head factor of the negligible-source state must not be kept after the floor inflow vanishes. In the usual physical-area convention $q=A_{\rm phys}C_d\sqrt{2\delta p/\rho}$, the equivalent formula is $Q_c=(2C_d^2A_{\rm phys}^2BH)^{1/3}$.

The quoted pure-plume law cannot be used unmodified down to the origin for a source with nonzero volume: it would incorrectly give zero flux there. A compatible finite-source example uses a virtual origin,

$$
q_p(h;Q)=\lambda B^{1/3}(h+h_0)^{5/3},\qquad
h_0=\left(\frac{Q}{\lambda B^{1/3}}\right)^{3/5}.
$$

It recovers the supplied pure-plume limit when $Q\to0$, and gives the same blocking threshold. The complete finite-$Q$ interface trajectory depends on that plume model, but the threshold needs only source-volume conservation and positive entrainment. For $Q>Q_c$, the assumed steady regime with a lower inflow no longer exists.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
