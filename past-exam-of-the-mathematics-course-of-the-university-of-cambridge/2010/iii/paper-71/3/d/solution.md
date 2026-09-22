<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let states $1$ and $2$ be just left and right of a [hydraulic bore](../../../../../../hydraulic-bore.md) moving at speed $s$, and let $[f]=f_2-f_1$. Integrating the conservative [prismatic-channel shallow water equations](../../../../../../prismatic-channel-shallow-water-equations.md) across it gives the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md)

$$
\boxed{s[A]=[Au],\qquad s[Au]=[Au^2+P],\qquad
A=\frac23h^{3/2},\quad P=\frac4{15}gh^{5/2}.}
$$

Equivalently the discharge in the [shock frame](../../../../../../shock-frame.md) is common on the two sides,

$$
j=A_1(u_1-s)=A_2(u_2-s),
\qquad
j^2\left(\frac1{A_1}-\frac1{A_2}\right)=P_2-P_1.
$$

Thus, for unequal positive depths,

$$
s=\frac{A_2u_2-A_1u_1}{A_2-A_1},\qquad
j^2=\frac{A_1A_2(P_2-P_1)}{A_2-A_1}.
$$

[Momentum](../../../../../../momentum.md) is conserved through the bore in this ideal model, but mechanical energy is dissipated; an energy-conservation jump must not be imposed as well.

For a stationary bore with rightward flow, $s=0$, $A_1u_1=A_2u_2>0$, and the momentum jump must still hold. A compressive [hydraulic jump](../../../../../../hydraulic-jump.md) has $h_2>h_1$ and

$$
\boxed{u_1-c_1>0>u_2-c_2,\qquad u_1+c_1>0,\quad u_2+c_2>0.}
$$

The $u-c$ [characteristic curves](../../../../../../characteristic-curve.md) approach the stationary bore from both sides: upstream flow is [supercritical flow](../../../../../../supercritical-flow.md), while downstream flow is [subcritical flow](../../../../../../subcritical-flow.md) using the local wave speed $c_i=\sqrt{2gh_i/3}$. The $u+c$ family travels downstream on both sides. These characteristic directions accompany, rather than replace, the two stationary conservation jumps.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
