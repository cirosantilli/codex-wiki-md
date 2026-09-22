<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a long finite blade with negligible under-blade flux, fluid accumulates upstream and escapes sideways around the ends. The [finite-blade side-drainage pile](../../../../../../finite-blade-side-drainage-pile.md) has $h\gg1$ in a broad upstream region, while its near wake is strongly depleted; far from the blade the incoming film still has thickness one. The schematic in the preceding figure shows the pile, incoming flow, and escape around the ends.

Away from the nose and end regions, the streamwise flux nearly cancels: $-h-h^3h_x/3\simeq0$. This is the deep part of the [infinite-blade gravity pile](../../../../../../infinite-blade-gravity-pile.md), so $h^3=9[x_N(y)-x]$ is the appropriate local profile. The hierarchy $1\ll x_N\ll\alpha$ makes streamwise variation much faster than lateral variation, while allowing lateral flow to carry away the integrated influx.

Set $I(y)=\int_0^{x_N(y)}h^4\,dx$ and $Q_y=\int_0^{x_N(y)}q_y\,dx$. Since $q_y=-h^3h_y/3=-(h^4)_y/12$ and the leading deep-pile profile vanishes at its nose, $Q_y=-I'/12$. Integrating steady conservation in $x$ gives $Q_y'=1$: the wall has zero normal flux, whereas the matched incoming film supplies flux $-1$ per unit blade length. Equivalently one can integrate to an upstream matching plane, where the moving-frame flux is exactly $-1$; this avoids incorrectly assigning zero incoming flux to the approximate zero-height nose. Symmetry gives $Q_y(0)=0$. Therefore

$$
\boxed{\frac{d}{dy}\int_0^{x_N}h^4\,dx=-12y.}
$$

At leading order the deep pile ends at $y=\pm\alpha$, so $I(\pm\alpha)=0$, giving $I=6(\alpha^2-y^2)$. Direct integration of the cubic profile yields $I=(3/7)9^{4/3}x_N^{7/3}$. Thus

$$
\boxed{x_N(y)=\frac{[126(\alpha^2-y^2)]^{3/7}}9,\qquad h(0^+,y)=[126(\alpha^2-y^2)]^{1/7}.}
$$

In particular $x_N(0)=O(\alpha^{6/7})\ll\alpha$ and $h(0,0)=O(\alpha^{2/7})\gg1$, confirming the assumed hierarchy. The local nose and tip regions are outside this leading deep-pile approximation.

Apply the [squeegee gap leakage flux](../../../../../../squeegee-gap-leakage-flux.md) with $\Delta p$ at most of order the largest pile height. A sufficient negligible-leakage criterion is

$$
\boxed{\frac{2\epsilon^{5/2}}{9\pi\sqrt{2\delta}}(126\alpha^2)^{1/7}\ll1,\qquad\epsilon\ll\delta\ll1.}
$$

The floor-driven $2\epsilon/3$ must also be small, as it is in this regime. In scaling form the additional restriction is **$\epsilon\ll\delta^{1/5}\alpha^{-4/35}$**. The total leakage divided by incoming volume flux has the same scaling; blade length does not introduce an extra factor of $\alpha$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
