<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $\nu<0$ and small negative $\mu$, the returning trajectory enters to the left of the bottleneck, crosses the region around $x=0$ slowly, and exits to the right. Its height contracts towards $y=0$ throughout because $\dot y=-\lambda y$. The local horizontal arrows point right everywhere. There is no [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md); the schematic global excursion then returns the trajectory to the incoming section, giving the stable [limit cycle](../../../../../../limit-cycle.md) shown in the negative-$\mu$, negative-$\nu$ panel.

For fixed $h>0$, the complete local bottleneck crossing takes

$$
\int_{-h}^h\frac{dx}{x^2-\mu}
=\frac2{\sqrt{-\mu}}\arctan\frac h{\sqrt{-\mu}}
=\frac\pi{\sqrt{-\mu}}-\frac2h+O(-\mu).
$$

The actual entry coordinate is near a fixed negative $\nu$. Replacing $-h$ by that entry removes only a bounded time as $\mu\to0^-$, and the global excursion also takes bounded time. Therefore

$$
\boxed{T\sim\frac\pi{\sqrt{-\mu}}.}
$$

This is the [inverse-square-root period law near a saddle-node bottleneck](../../../../../../inverse-square-root-period-law-near-a-saddle-node-bottleneck.md). The coefficient $\pi$ assumes fixed negative $\nu$, or more generally $-\nu/\sqrt{-\mu}\to\infty$. In a joint approach to the codimension-two point, the actual local time is $[\arctan(h/k)-\arctan(\nu/k)]/k$, $k=\sqrt{-\mu}$. If $\nu/k\to-C$, the coefficient is $\pi/2+\arctan C$ instead; at entry $\nu=0$ it is $\pi/2$. The fixed-negative-$\nu$ law is not uniform over all joint parameter paths.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
