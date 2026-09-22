<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Normalize all fluxes by $\pi$, rather than including that factor in only some of them. The specific plume [volume flux](../../../../../../volumetric-flow-rate.md), [momentum flux](../../../../../../momentum-flux.md) and [buoyancy flux](../../../../../../buoyancy-flux.md) are

$$
\boxed{Q=b^2w,\qquad M=b^2w^2,\qquad B=b^2wg'=B_s.}
$$

The ambient transport is $-Q$ and its specific [momentum flux](../../../../../../momentum-flux.md) is

$$
M_a=(R^2-b^2)v^2=\frac{Q^2}{R^2-Q^2/M}.
$$

Put $s=b^2/R^2=Q^2/(R^2M)$, with $0<s<1$. The total specific [momentum flux](../../../../../../momentum-flux.md) is

$$
J=M+M_a=\frac{M}{1-s},\qquad b=\frac{Q}{\sqrt M},\qquad w=\frac MQ,\qquad g'=\frac{B_s}{Q}.
$$

The first differential equation follows immediately from relative-speed [fluid entrainment](../../../../../../fluid-entrainment.md):

$$
\boxed{Q'=\frac{2\alpha\sqrt M}{1-s}.}
$$

For the second, differentiate $J=M/(1-s)$ and use $s'=2sQ'/Q-sM'/M$. Since $J'=b^2g'=B_sQ/M$, this yields

$$
\boxed{(1-2s)M'=\frac{B_sQ}{M}(1-s)^2-\frac{2Q}{R^2}Q'.}
$$

This is the requested two-equation system, with $B=B_s$ and zero total [volume flux](../../../../../../volumetric-flow-rate.md) as the additional conservation conditions. Near the pure source, $Q,M\to0$ and $s\to0$. Eliminating height in that limit gives

$$
\frac{dM}{dQ}\sim\frac{B_sQ}{2\alpha M^{3/2}},\qquad M^{5/2}\sim\frac{5B_s}{8\alpha}Q^2.
$$

The zero [integration](../../../../../../integral.md) constant selects a [pure plume](../../../../../../pure-plume.md); a nonzero imposed source [momentum](../../../../../../momentum.md) would select a different branch and generally a different turning height. The leading radius is $b\sim6\alpha z/5$, which recovers the unconfined pure-plume limit near the source.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
