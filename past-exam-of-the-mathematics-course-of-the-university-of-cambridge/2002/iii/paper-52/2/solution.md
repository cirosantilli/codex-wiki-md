<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\theta=T-T_0>0$ and $\theta_1=T_1-T_0$. The aperture spans the enclosure's depth $H$, so the incoming [volume flux](../../../../../volumetric-flow-rate.md), equal to the outgoing [volume flux](../../../../../volumetric-flow-rate.md), is

$$
q=\frac{Hh}{2}\,c\sqrt{g\beta h\theta}.
$$

Only one of these equal exchange fluxes multiplies the [temperature](../../../../../temperature.md) difference in the [heat](../../../../../heat.md) budget: incoming fluid brings $qT_0$, outgoing fluid removes $qT$. With constant [mass density](../../../../../density.md) and [specific heat capacity](../../../../../specific-heat-capacity.md), those factors cancel and the [well-mixed ventilation temperature balance](../../../../../well-mixed-ventilation-temperature-balance.md) is

$$
H^3\dot\theta=-q\theta,\qquad
\dot\theta=-k\theta^{3/2},\qquad
k=\frac{c h^{3/2}\sqrt{g\beta}}{2H^2}.
$$

Integrating from $\theta_1$ gives

$$
\boxed{T(t)=T_0+\frac{T_1-T_0}{\left[1+\dfrac{c h^{3/2}\sqrt{g\beta(T_1-T_0)}}{4H^2}\,t\right]^2}.}
$$

The cooling is algebraic rather than exponential because the buoyancy-driven [single-opening exchange flow](../../../../../single-opening-exchange-flow.md) weakens as its driving [reduced gravity](../../../../../reduced-gravity-split.md) decreases. The formula assumes negligible wall [heat capacity](../../../../../heat-capacity.md), no heat input, the specified aperture geometry, and a uniform interior [temperature](../../../../../temperature.md) maintained by mixing.

With a low-level opening, the dense incoming cold fluid tends to spread along the floor instead of falling through the warm interior. A cold lower layer and warm upper layer develop, giving [stable density stratification](../../../../../stable-density-stratification.md). The incoming fluid can short-circuit back out through the low opening after that layer occupies it, leaving warm fluid above poorly ventilated. Thus the uniform-temperature assumption is generally inappropriate: cooling becomes vertically nonuniform and substantially slower for the upper warm fluid. If mixing were artificially maintained, the same lumped budget would still apply; it is the loss of that assumption, rather than a reversal of [buoyancy](../../../../../buoyancy.md), that changes the physical outcome.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [Section A](../section-a.md)
3. [Paper 52](../../paper-52-split.md)
4. [Iii](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
