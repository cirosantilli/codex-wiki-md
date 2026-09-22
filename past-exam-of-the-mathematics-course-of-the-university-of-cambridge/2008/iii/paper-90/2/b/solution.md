<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The occupied cross-sectional area and interface width are

$$
A(h)=\int_0^h z\,dz=\frac{h^2}{2},\qquad b(h)=h.
$$

The incoming [volume flux](../../../../../../volumetric-flow-rate.md) per unit channel length is $hw_e$. [Volume conservation](../../../../../../volume-conservation.md) therefore gives $A_t+(Au)_x=hw_e$. Ambient fluid carries no excess [mass density](../../../../../../density.md), so integrating the excess-[mass density](../../../../../../density.md) balance gives $(Ag')_t+(Aug')_x=0$. These two equations imply dilution of the [reduced gravity](../../../../../../reduced-gravity-split.md), even though total integrated [buoyancy](../../../../../../buoyancy.md) is conserved.

The integrated horizontal [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force, divided by the reference [mass density](../../../../../../density.md), is

$$
\int_0^h g'(h-z)z\,dz=\frac{g'h^3}{6}.
$$

The prismatic walls contribute no axial component of pressure force. Since ambient fluid enters with zero horizontal [velocity](../../../../../../velocity.md), it supplies no horizontal [momentum flux](../../../../../../momentum-flux.md). Thus the [entraining shallow-water current in a triangular channel](../../../../../../entraining-shallow-water-current-in-a-triangular-channel.md) obeys the conservative equations

$$
\boxed{
\begin{aligned}
\partial_t\left(\frac{h^2}{2}\right)+\partial_x\left(\frac{h^2u}{2}\right)&=hw_e,\\
\partial_t\left(\frac{h^2u}{2}\right)+\partial_x\left(\frac{h^2u^2}{2}+\frac{g'h^3}{6}\right)&=0,\\
\partial_t\left(\frac{h^2g'}{2}\right)+\partial_x\left(\frac{h^2ug'}{2}\right)&=0.
\end{aligned}}
$$

To put them in primitive form, let $D=\partial_t+u\partial_x$ be the [material derivative](../../../../../../material-derivative.md). The volume equation gives $Dh+(h/2)u_x=w_e$. Subtracting $u$ times the volume equation from the momentum equation, and $g'$ times it from the [buoyancy](../../../../../../buoyancy.md) equation, yields

$$
\boxed{
\begin{aligned}
Dh+\frac h2u_x&=w_e,\\
Du+g'h_x+\frac h3g'_x&=-\frac{2uw_e}{h},\\
Dg'&=-\frac{2g'w_e}{h}.
\end{aligned}}
$$

The momentum source is the acceleration of newly entrained ambient fluid, not bed drag. The source in the [reduced gravity](../../../../../../reduced-gravity-split.md) equation describes mixing with ambient fluid of zero excess [mass density](../../../../../../density.md). In particular, the rectangular-channel coefficients cannot be used: the triangular area produces both $h/2$ in the depth equation and $h/3$ in the [buoyancy](../../../../../../buoyancy.md)-gradient force.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
