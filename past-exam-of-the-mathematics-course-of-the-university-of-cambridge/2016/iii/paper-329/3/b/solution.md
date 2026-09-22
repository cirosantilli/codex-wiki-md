<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an infinite blade, the steady moving-frame flux is constant and its upstream value is $-1$. The [infinite-blade gravity pile](../../../../../../infinite-blade-gravity-pile.md) therefore satisfies $-h-h^3h_x/3=-1$, or $h_x=-3(h-1)/h^3$. Integrating gives

$$
\boxed{X(h)=\frac{h^3}{9}+\frac{h^2}{6}+\frac h3+\frac13\log(h-1)=x_0-x,\qquad h>1.}
$$

An additive constant in $X$ simply shifts $x_0$. The head at the blade, and hence $x_0$, must supply the pressure difference that makes the flux beneath the blade equal to the incoming flux. For $x_0\gg1$ the deep part has $h\simeq[9(x_0-x)]^{1/3}$, followed by a smooth transition to $h=1$ with $h-1$ exponentially small, proportional to $e^{-3x}$. Thus $x_0$ is an approximate nose coordinate, not a sharp front of the exact solution.

Near the rounded edge the [parabolic lubrication gap](../../../../../../parabolic-lubrication-gap.md) is $d(x)=\epsilon+\delta-\sqrt{\delta^2-x^2}\simeq\epsilon+x^2/(2\delta)$. In the blade frame the floor moves at $-1$ and the blade is stationary. The [Couette-Poiseuille flow in a thin gap](../../../../../../couette-poiseuille-flow-in-a-thin-gap.md) has flux $q_x=-d/2-d^3p_x/12$. Let $J=-q_x$ be positive leakage towards the rear, and let $\Delta p=p_{\rm ahead}-p_{\rm rear}>0$. The narrow-gap integrals are

$$
I_2=\int_{-\infty}^{\infty}\frac{dx}{d^2}=\frac{\pi\sqrt{2\delta}}{2\epsilon^{3/2}},\qquad I_3=\int_{-\infty}^{\infty}\frac{dx}{d^3}=\frac{3\pi\sqrt{2\delta}}{8\epsilon^{5/2}}.
$$

Integrating the pressure gradient gives $\Delta p=12JI_3-6I_2$, so the [squeegee gap leakage flux](../../../../../../squeegee-gap-leakage-flux.md) is

$$
\boxed{J\simeq\frac{2\epsilon}{3}+\frac{2\epsilon^{5/2}}{9\pi\sqrt{2\delta}}\Delta p.}
$$

The first term is the floor-driven contribution. For the steady infinite blade, $J=1$, so $\Delta p\simeq9\pi\sqrt{2\delta}/(2\epsilon^{5/2})$. The [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) difference is the height difference at the two sides. A fully developed rear layer of thickness $h_-$ has moving-frame flux $-h_-$; hence **$h_-=1$**, and

$$
\boxed{h(0^+)\simeq\frac{9\pi\sqrt{2\delta}}{2\epsilon^{5/2}}.}
$$

The large head eventually forces all the arriving film beneath an infinite blade. Taking a perfectly closed gap instead would eliminate this steady state.

<a id="3/b/image-infinite-blade-height-profile-and-schematic-finite-blade-pile-with-sideways-drainage"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-329-squeegee-flow.png)

**[Figure 2](#3/b/image-infinite-blade-height-profile-and-schematic-finite-blade-pile-with-sideways-drainage). Infinite-blade height profile and schematic finite-blade pile with sideways drainage**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
