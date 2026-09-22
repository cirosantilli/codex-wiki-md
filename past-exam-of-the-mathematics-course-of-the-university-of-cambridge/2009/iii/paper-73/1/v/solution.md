<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The mobile fluid volume per unit well length includes the [porosity](../../../../../../porosity.md):

$$
V(t)=\phi\int_0^{ut/\phi}h(x,t)\,dx.
$$

Integrating the [residual-trapping attenuation of a porous current](../../../../../../residual-trapping-attenuation-of-a-porous-current.md) gives, for $0\leq s<1$,

$$
\boxed{V(t)=\frac{Q\tau}{1-s}\left(e^{-st/\tau}-e^{-t/\tau}\right).}
$$

This is mobile volume in the current; retained fluid outside its mobile thickness is not counted. Since $h_t=-h/\tau$ in the thinning region, the rate of accumulation of immobile retained volume is $\dot V_r=sV/\tau$. Direct differentiation verifies $\dot V+\dot V_r=Qe^{-t/\tau}$, so the mobile-volume expression obeys the overall injection balance.

Without [capillary residual trapping](../../../../../../capillary-residual-trapping.md), $s=0$ gives $V=Q\tau(1-e^{-t/\tau})$. The limiting expression as $s\to1$ is $V=Qt e^{-t/\tau}$, though the local thinning equation degenerates at exactly $s=1$. Both limits provide useful consistency checks.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
