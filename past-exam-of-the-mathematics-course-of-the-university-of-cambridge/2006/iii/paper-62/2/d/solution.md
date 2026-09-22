<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume $V>0$ and that its derivatives do not change substantially over the field interval traversed in the estimate. With initially negligible [kinetic energy](../../../../../../kinetic-energy.md), $H^2\simeq V/(3M_{\rm Pl}^2)$. The force $-V_{,\phi}$ changes the field [velocity](../../../../../../velocity.md) on the [Hubble friction](../../../../../../hubble-friction.md) time. Keeping $H$ and $V_{,\phi}$ approximately constant for that local estimate, and starting at rest, solves the field equation explicitly:

$$
\dot\phi(t)=-\frac{V_{,\phi}}{3H}(1-e^{-3H\Delta t}),\qquad \Delta t=t-t_i.
$$

After one [Hubble time](../../../../../../hubble-time.md),

$$
\frac{\dot\phi^2}{V}\simeq\frac{M_{\rm Pl}^2V_{,\phi}^2}{3V^2}(1-e^{-3})^2.
$$

Writing $A=M_{\rm Pl}^2V_{,\phi}^2/V^2$, the condition $A<1$ keeps this kinetic-to-potential ratio below about $0.31$, comfortably inside the inflationary bound. Integrating once more gives the fractional potential change estimate

$$
\frac{|\Delta V|}{V}\simeq A\left[1-\frac{1-e^{-3}}3\right]\simeq0.683A
$$

over the same interval. Thus the characteristic time for an order-one potential change is $H^{-1}/A$, up to constants of order one. The requested local Hubble-timescale criterion is

$$
\boxed{M_{\rm Pl}^2\frac{V_{,\phi}^2}{V^2}\lesssim1.}
$$

Using a strict inequality with one as the order-one threshold is conventional; its coefficient is not an exact universal end-of-inflation bound. Much smaller $A$ gives the controlled slow-roll regime and many [Hubble times](../../../../../../hubble-time.md) of [cosmic inflation](../../../../../../cosmic-inflation-split.md) if the bounds persist.

After the transient in [relaxation to the slow-roll attractor](../../../../../../relaxation-to-the-slow-roll-attractor.md), $3H\dot\phi\simeq-V_{,\phi}$. Differentiating this approximate relation gives

$$
\frac{\ddot\phi}{H\dot\phi}\simeq-\frac{V_{,\phi\phi}}{3H^2}-\frac{\dot H}{H^2}\simeq-\eta_V+\epsilon_V,
\qquad \epsilon_V=\frac{M_{\rm Pl}^2}{2}\left(\frac{V_{,\phi}}V\right)^2,\quad \eta_V=M_{\rm Pl}^2\frac{V_{,\phi\phi}}V.
$$

Therefore the standard sufficient conditions for negligible acceleration throughout slow roll are $\epsilon_V\ll1$ and

$$
\boxed{\left|M_{\rm Pl}^2\frac{V_{,\phi\phi}}V\right|\ll1.}
$$

The [absolute value](../../../../../../absolute-value.md) matters: large negative curvature also drives rapid evolution. The more precise local acceleration criterion is $|\eta_V-\epsilon_V|\ll1$, with the usual separate smallness conditions avoiding a tuned cancellation. If a field starts exactly at rest on a nonzero slope, its initial acceleration is not negligible; the displayed exponential transient describes its approach to the attractor.

These are local timescale and slow-roll conditions, rather than a global duration theorem from derivatives at a single point. A smooth potential can have a narrow flat shoulder followed by a steep drop, ending [cosmic inflation](../../../../../../cosmic-inflation-split.md) soon despite small starting derivatives. The conditions must hold over the traversed interval. This is the additional smooth-evolution assumption implicit in the estimate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
